# Stock Price Forecasting Using Deep Learning

## Project Overview

This project focuses on forecasting the stock price of Infosys Limited (INFY) using deep learning techniques. Historical weekly stock price data containing Open, High, Low, Close, and Volume features was analysed to identify trends, patterns, and temporal relationships in stock price movements.

Five deep learning models were developed and compared:

- Recurrent Neural Network (RNN)
- Gated Recurrent Unit (GRU)
- Long Short-Term Memory (LSTM)
- Convolutional Neural Network (CNN)
- CNN-LSTM Hybrid Model

The models were evaluated using chronological data splitting and walk-forward validation to provide a realistic time-series forecasting evaluation.

## Objectives

- Analyse historical Infosys stock price behaviour.
- Perform exploratory data analysis on stock price and trading volume.
- Preprocess and normalize the historical stock data.
- Create sequential input data for deep learning models.
- Develop and compare multiple deep learning architectures.
- Evaluate model performance using forecasting metrics.
- Forecast the next week's Infosys stock price.
- Identify the best-performing deep learning model.

## Dataset

The dataset contains historical weekly stock price observations for Infosys Limited (INFY).

### Features

Date: Trading week date 
Open: Opening stock price 
High: Highest price during the week 
Low: Lowest price during the week 
Close: Closing stock price 
Volume: Number of shares traded

The dataset was obtained from Yahoo Finance and contains weekly observations from 2011 to 2026.

## Methodology

The project follows these major steps:

1. Data Collection
2. Data Cleaning
3. Date Formatting and Chronological Ordering
4. Exploratory Data Analysis
5. Feature Selection
6. Min-Max Normalization
7. Time-Series Sequence Creation
8. Chronological Train-Test Split
9. Walk-Forward Validation
10. Deep Learning Model Development
11. Model Evaluation
12. Next-Week Stock Price Forecasting

## Exploratory Data Analysis

The analysis includes:

- Stock price trend analysis
- Return analysis
- Volatility analysis
- Lag relationship analysis
- Rolling mean and rolling standard deviation
- Distribution analysis
- Stock price movement analysis

## Deep Learning Models

### RNN

Recurrent Neural Network designed to learn sequential and temporal relationships in stock price data.

### GRU

Gated Recurrent Unit designed to capture temporal dependencies using update and reset gates with fewer parameters than LSTM.

### LSTM

Long Short-Term Memory network designed to learn long-term dependencies in sequential financial data.

### CNN

Convolutional Neural Network adapted for time-series forecasting to extract local patterns and short-term fluctuations.

### CNN-LSTM

A hybrid architecture combining CNN for local feature extraction and LSTM for learning long-term temporal dependencies.

## Model Evaluation

The models were evaluated using:

- Mean Absolute Error (MAE)
- Root Mean Square Error (RMSE)
- Mean Absolute Percentage Error (MAPE)
- Prediction Accuracy

Lower MAE, RMSE, and MAPE indicate better performance, while higher accuracy indicates better forecasting performance.

## Results

RNN:
  MAE = 40.9568
  RMSE = 52.8356
  MAPE = 2.75%
  Accuracy = 97.25%

GRU:
  MAE = 43.1909
  RMSE = 55.8884
  MAPE = 2.91%
  Accuracy = 97.09%

LSTM:
  MAE = 44.5015
  RMSE = 56.7237
  MAPE = 3.01%
  Accuracy = 96.99%

CNN:
  MAE = 42.7647
  RMSE = 55.1892
  MAPE = 2.80%
  Accuracy = 97.20%

CNN-LSTM:
  MAE = 41.8320
  RMSE = 53.8368
  MAPE = 2.80%
  Accuracy = 97.20%

### Best Performing Model

The RNN model achieved the best overall performance, recording the lowest MAE, RMSE, and MAPE and the highest prediction accuracy of 97.25%.

## Next-Week Forecast

The reported next-week forecasts were:
RNN:
  Current Price = 1535.80
  Predicted Price = 1547.97
  Predicted Return = 0.79%

GRU:
  Current Price = 1535.80
  Predicted Price = 1549.79
  Predicted Return = 0.91%

LSTM:
  Current Price = 1535.80
  Predicted Price = 1563.44
  Predicted Return = 1.80%

CNN:
  Current Price = 1535.80
  Predicted Price = 1528.34
  Predicted Return = -0.49%

CNN-LSTM:
  Current Price = 1535.80
  Predicted Price = 1548.47
  Predicted Return = 0.83%

The forecasts generally indicate a moderate upward expectation, although individual models show different short-term movements.

## Key Findings

- Infosys stock shows an overall increasing trend with short-term fluctuations.
- Historical stock prices contain temporal patterns suitable for time-series forecasting.
- All five deep learning models achieved accuracy above 96%.
- RNN achieved the best overall performance among the tested models.
- CNN-LSTM also provided strong forecasting performance.
- The next-week forecasts generally indicate a slight increase in the stock price.

## Limitations

- The study uses only historical stock price and volume information.
- Economic conditions, company-specific factors, and market news were not included.
- Weekly data may not capture short-term daily market movements.
- Only selected deep learning architectures were evaluated.

## Future Scope

Future improvements could include:

- Adding technical indicators.
- Incorporating economic and market factors.
- Including market sentiment and news data.
- Testing Transformer and attention-based architectures.
- Applying the methodology to multiple companies and sectors.
- Exploring ensemble modelling approaches.
- Using daily stock price data for more detailed forecasting.
