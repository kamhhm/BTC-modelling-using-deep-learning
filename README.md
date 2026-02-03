# Bitcoin Price Prediction: LSTM vs Linear Regression

A machine learning pipeline comparing LSTM (Long Short-Term Memory) neural networks with Linear Regression for predicting Bitcoin market movements.

## Research Question

> Is the LSTM machine learning algorithm more effective than linear regression in predicting bitcoin market movements?

## Results

**LSTM outperforms Linear Regression by 86.3%** on unseen test data.

| Metric | Linear Regression | LSTM |
|--------|-------------------|------|
| Average Error | $23,765 | $3,257 |
| MSE | 583.97 | 15.02 |
| R-squared | -43.72 | -0.22 |

*All metrics evaluated on held-out test data only (proper ML evaluation).*

## ML Best Practices

This project follows fundamental machine learning principles:

- **70/15/15 Train/Validation/Test Split**: Ensures unbiased evaluation
- **No Data Leakage**: Test set is never seen during training or validation
- **Temporal Ordering Preserved**: Critical for time-series forecasting
- **Separate Validation Set**: Used for hyperparameter tuning during LSTM training

## Project Structure

```
bitcoin-ml-pipeline/
├── bitcoin_ml_pipeline.ipynb  # Main Jupyter notebook
├── data/
│   ├── bitcoin_prices.csv     # Bitcoin price dataset (565 days)
│   └── README.md              # Data documentation
├── requirements.txt           # Python dependencies
└── README.md                  # This file
```

## Quick Start

```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/bitcoin-ml-pipeline.git
cd bitcoin-ml-pipeline

# Create virtual environment
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook bitcoin_ml_pipeline.ipynb
```

## Models Compared

### Linear Regression
- Simple, interpretable baseline model
- Equation: Y = θ₂X + θ₁
- Assumes linear relationship between time and price

### LSTM (Long Short-Term Memory)
- Deep learning model designed for sequential data
- Captures long-term dependencies through gating mechanisms
- Uses 60-day lookback window for predictions

## Dataset

565 days of Bitcoin prices from **November 2020 to May 2022**, covering:
- Bitcoin's rise to ~$60,000
- Significant market volatility
- Major corrections and recoveries

## Tech Stack

- **Python 3.11+**
- **TensorFlow/Keras** - LSTM implementation
- **Scikit-learn** - Linear Regression and metrics
- **Pandas/NumPy** - Data manipulation
- **Matplotlib** - Visualizations

## References

- [Understanding LSTM Networks](https://colah.github.io/posts/2015-08-Understanding-LSTMs/)
- [Scikit-learn Linear Regression](https://scikit-learn.org/stable/modules/linear_model.html)
- [TensorFlow LSTM Documentation](https://www.tensorflow.org/api_docs/python/tf/keras/layers/LSTM)
