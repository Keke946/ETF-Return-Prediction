# ETF Return Prediction Project

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
