# ETF Return Prediction Project

This project aims to predict the forward close-to-close return for 16 ETFs using historical data.

I firstly applied a **Vector AutoRegression (VAR)** model as a baseline multivariate time-series model. Then I chose a more advanced multi-factor machine learning model **XGBoost**, to provide some better predictions.

My prediction target is:  
> Given all information up to time `t`, predict the return from `t` to `t+1` (close-to-close).

Performance is evaluated based on **cumulative cross-sectional Information Coefficient (IC)**, both in-sample and out-of-sample.

ETF symbols: ['DIA', 'IWM', 'QQQ', 'SPY', 'VXX', 'XLB', 'XLC', 'XLE', 'XLF', 'XLI','XLK', 'XLP', 'XLRE', 'XLU', 'XLV', 'XLY']

This repository contains all files related to the ETF return prediction project, including data processing, model training, hyperparameter tuning, and strategy backtesting.

## Project Structure📁📁📁

- `data/`:  
  - Original ETF historical CSVs  
  - Cleaned and merged datasets used for modeling

- `models/`:  
  Stores the hyperparameter sets used for each XGBoost model

- `results/`:  
  Contains prediction outputs and backtest return series

- `figures/`:  
  Includes return trend plots and IC visualizations

- `optuna_study/`:  
  Saved Optuna optimization studies (for reproducibility)

- `main.ipynb`:  
  The full pipeline notebook (feature engineering, modeling, evaluation, backtesting)

## How to Run🚀🚀🚀

1. Place all original ETF CSVs in `data/original_data/`
2. Open and run `main.ipynb` from top to bottom
3. Backtest results and prediction outputs will be saved to `results/`
