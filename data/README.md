# Bitcoin Price Data

This folder contains the Bitcoin price dataset used for the ML pipeline.

## Dataset Description

- **File**: `bitcoin_prices.csv`
- **Period**: November 2020 to May 2022 (Bitcoin's peak relevancy)
- **Features**:
  - `Day`: Sequential day number (1-565)
  - `Open`: Opening price in thousands of USD (e.g., 13.781 = $13,781)

## Data Source

This is dummy data based on historical Bitcoin prices during its most volatile period. 
Replace with actual data from sources like:
- CoinGecko API
- Coinbase
- Yahoo Finance
- Kaggle Bitcoin datasets

## Notes

- Prices are in thousands to prevent float overflow issues
- The dataset captures Bitcoin's rise to ~$60k and subsequent volatility
