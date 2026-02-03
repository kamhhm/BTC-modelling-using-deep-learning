# Bitcoin Price Prediction: LSTM vs LR

A machine learning pipeline comparing LSTM (Long Short-Term Memory) neural networks with Linear Regression as a baseline model.

Result - **LSTM outperforms Linear Regression by 86.3%** on unseen test data.

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
