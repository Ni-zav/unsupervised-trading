# Unsupervised Trading Strategy Experiment

An experimental implementation exploring unsupervised machine learning applications to portfolio construction, specifically using K-means clustering to group assets with similar characteristics.

## Overview

This project attempts to implement a systematic approach that:
1. Downloads historical SP500 stocks price data
2. Processes basic features and technical indicators
3. Filters for liquidity and aggregates data monthly
4. Analyzes returns across different time horizons
5. Incorporates Fama-French factors for risk analysis
6. Tests K-means clustering for asset grouping
7. Attempts portfolio construction using optimization
8. Compares results with market benchmark

## Requirements

Required Python packages (Python 3.8+ recommended):

```
pandas>=1.2.0
numpy>=1.19.0
matplotlib>=3.3.0
statsmodels>=0.12.0
pandas_datareader>=0.9.0
yfinance>=0.1.63
scikit-learn>=0.24.0
PyPortfolioOpt>=1.4.0
jupyter>=1.0.0
```

## Setup & Usage

This is a Jupyter notebook-based implementation:

1. Set up environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
```

2. Run Jupyter:
```bash
jupyter notebook notebook.ipynb
```

3. The notebook contains:
   - Data loading and preprocessing
   - Feature calculation steps
   - Clustering implementation
   - Simple portfolio construction attempt

## Implementation Details

The experiment uses:

- **Data Processing:**
  - Basic volatility metrics
  - Common technical indicators
  - Simple liquidity filtering

- **Analysis:** 
  - Multiple return horizons
  - Factor analysis with Fama-French data
  - Basic momentum and volatility metrics

- **Methods:**
  - Basic K-means clustering implementation
  - Simple portfolio optimization attempts
  - Monthly rebalancing tests

## Limitations

This is an experimental implementation with several limitations:
- No transaction costs considered
- Simplified risk management
- Basic portfolio constraints
- Limited backtesting framework
- Not optimized for real-world trading

## Data Sources

- Fama-French factors: Kenneth French's Data Library
- Stock data: Yahoo Finance API
- Index constituents: Wikipedia

## Important Disclaimer

This is an educational experiment only. The implementation has not been thoroughly tested for real trading conditions. Do not use for actual investment decisions. All trading carries significant risk of loss. Past performance does not indicate future results.
