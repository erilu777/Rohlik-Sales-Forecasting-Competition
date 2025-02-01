# Rohlik Sales Forecasting Challenge

## Overview
Time series forecasting solution for the [Rohlik Sales Forecasting Challenge on Kaggle](https://www.kaggle.com/competitions/rohlik-sales-forecasting-challenge-v2)

## Setup
1. Download competition data from [Kaggle](https://www.kaggle.com/competitions/rohlik-sales-forecasting-challenge-v2/data)
2. Place all .csv files in a `data/` directory
3. Run the notebook `rohlik_sales_forecast.ipynb`

## Approach
- Feature engineering:
  - Time-based features (day, month, year)
  - Lag features (7, 14, 28, 365 days)
  - Product category hierarchies
- Model: LightGBM with weighted MAE optimization
- Validation: Used last 14 days of May 2024 as validation set

## Results
- Validation WMAE: 24.96
