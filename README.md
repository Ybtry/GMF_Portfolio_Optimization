# 10 Academy: Time Series Forecasting for Portfolio Management

## Project Overview
This project aims to apply time series forecasting to historical financial data for optimizing portfolio management strategies, as a Financial Analyst at GMF Investments.

### Business Objective
To predict market trends, optimize asset allocation, and enhance portfolio performance for clients by leveraging advanced time series forecasting models.

### Tasks Completed
- **Task 1: Preprocess and Explore the Data**
  - Fetched historical data for TSLA, BND, and SPY from YFinance.
  - Performed data cleaning, including handling missing values.
  - Conducted Exploratory Data Analysis (EDA) by visualizing prices, returns, and volatility.
  - Analyzed stationarity using the Augmented Dickey-Fuller (ADF) test, confirming TSLA prices are non-stationary and returns are stationary.
  - Calculated foundational risk metrics like annualized returns, volatility, Sharpe Ratio, and Value at Risk (VaR).

**Task 2: Model Development and Evaluation**
In this task, we focused on developing and evaluating two different time series models to forecast the adjusted close price of Microsoft (MSFT) stock. The goal was to compare their performance and select the best model for future portfolio optimization.

Models Developed
ARIMA Model: An AutoRegressive Integrated Moving Average (ARIMA) model was developed using the pmdarima library. This model served as a baseline to forecast future stock prices based on historical data.

PyTorch LSTM Model: A deep learning model using a Long Short-Term Memory (LSTM) neural network was built with the PyTorch framework. LSTMs are well-suited for capturing complex, non-linear patterns in sequential data like stock prices.

Model Performance Comparison
The performance of both models was evaluated on a test dataset using key metrics: Root Mean Squared Error (RMSE), Mean Absolute Error (MAE), and Mean Absolute Percentage Error (MAPE).

Metric	ARIMA Model	PyTorch LSTM Model
RMSE	34.94	17.88
MAE	29.44	14.54
MAPE	6.82%	3.31%

Export to Sheets
Conclusion
The PyTorch LSTM model demonstrated significantly better performance, with a much lower error across all metrics. This indicates that the LSTM model is more accurate for forecasting Microsoft's stock price in this project. We will proceed with the LSTM model for subsequent tasks.

New Dependencies
To run the updated code in this task, the following libraries are required:

torch

torchvision

torchaudio

pmdarima
---