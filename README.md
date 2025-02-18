## Overview
This project focuses on forecasting Bitcoin’s daily closing prices using neural networks and time series analysis techniques. The dataset consists of minute-level Bitcoin price data from January 1, 2021, to March 1, 2022. The model is trained to predict the closing prices for the last ten days of February 2022 using historical trends.

## Objectives
- Process and clean Bitcoin price data for accurate time series forecasting.
- Convert Unix timestamps to human-readable datetime format.
- Resample high-frequency data to daily closing prices to improve efficiency.
- Engineer time-based features to capture temporal dependencies.
- Train and evaluate a neural network model for price forecasting.
- Compare the performance of LSTM and ARIMA models using standard evaluation metrics.

## Features
1. **Data Preprocessing**:
   - Converted timestamps from Unix format to standard datetime.
   - Resampled minute-level data to daily closing prices to focus on long-term trends.
   - Identified and handled missing values using interpolation.
   - Engineered additional features such as `day_of_week`, `month`, and `year` to capture seasonal effects.

2. **Exploratory Analysis**:
   - Analyzed trading patterns and volatility across different timeframes.
   - Investigated the impact of lookback window size on model accuracy.

3. **Model Development**:
   - Implemented an LSTM-based deep learning model for sequential forecasting.
   - Applied ARIMA as a statistical benchmark model for comparison.

4. **Model Evaluation**:
   - Compared LSTM and ARIMA using Mean Absolute Error (MAE), Root Mean Squared Error (RMSE), and Mean Absolute Percentage Error (MAPE).
   - Evaluated training and inference time for both models.

5. **Forecasting**:
   - Predicted Bitcoin prices for the last ten days of February 2022.

## Results
- LSTM provided better accuracy than ARIMA, achieving lower MAE and MAPE values.
- ARIMA was computationally efficient with significantly lower training and inference time.
- The choice between LSTM and ARIMA depends on whether accuracy or speed is prioritized.

## Tools and Technologies
- **Languages**: Python
- **Libraries**: TensorFlow, scikit-learn, statsmodels, pandas, matplotlib
- **Techniques**: Time Series Analysis, ARIMA, LSTM, Feature Engineering

## Files Included
1. `Bitcoin-Time-Series-Forecasting.ipynb`: Jupyter Notebook containing data preprocessing, model training, and evaluation.
2. `Project Report.pdf`: Detailed LaTeX report discussing methodology and results.
3. `lookback_analysis.csv`: Analysis of different lookback periods and their impact on model performance.
4. `LSTM_vs_ARIMA_Comparison.csv`: Comparison of LSTM and ARIMA models based on accuracy and computational efficiency.
5. `bitcoin_data.csv.zip`: The dataset of Bitcoin prices and other features.

## How to Use
1. Clone the repository:
   ```bash
   git clone https://github.com/TasosFotiadis/Time-Series-Forecasting-For-Bitcoin.git
   cd Time-Series-Forecasting-For-Bitcoin
