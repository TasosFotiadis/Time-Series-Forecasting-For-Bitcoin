# Time-Series-Forecasting-For-Bitcoin
# Bitcoin Price Prediction Using Neural Networks

## Neuro-Fuzzy Computing Final Project

This repository contains a project on Bitcoin price forecasting using neural networks and time series analysis. The objective is to predict the daily closing price of Bitcoin based on historical data. The project was completed as part of the Neuro-Fuzzy Computing course.

---

## Project Structure

- `Bitcoin-Time-Series-Forecasting-Project` – Jupyter Notebook containing data preprocessing, model training, and predictions.
- `Project Report.pdf` – Detailed LaTeX report discussing methodology, results, and conclusions.
- `bitcoin_data.csv.zip` - Historical Bitcoin price data from January 1, 2021, to March 1, 2022.
- `LSTM_vs_ARIMA_Comparison.csv` - Comparison of LSTM and ARIMA models based on MAE, RMSE, MAPE, training, and inference time
- `lookback_analysis.csv` - Analysis of different lookback periods for time series forecasting
- `LICENSE` – Project license.

---

## Methodology

### Dataset
- The dataset consists of Bitcoin price data at a minute-level frequency.
- Data is sourced from January 1, 2021, to March 1, 2022.
- The target variable is the daily closing price of Bitcoin.
- Preprocessing steps include:
  - Conversion of timestamps from Unix format to human-readable datetime.
  - Resampling to daily closing prices to focus on long-term trends.
  - Handling of missing values through interpolation if necessary.
  - Feature engineering with additional time-based variables to enhance model performance.

### Neural Network Model
- Time series forecasting techniques are applied using a neural network-based approach.
- The model is trained on historical data to predict Bitcoin prices.
- The performance is evaluated by forecasting prices for the last ten days of February 2022.


