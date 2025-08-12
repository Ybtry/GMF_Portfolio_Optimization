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
**Task 3: Portfolio Optimization and Strategy Backtesting**

This phase successfully implemented the core components of MPT, including:

Data Collection: Gathered historical adjusted close prices for a portfolio of four major technology stocks: MSFT, AAPL, GOOG, and AMZN.

Efficient Frontier Simulation: Used a Monte Carlo simulation with 50,000 random portfolios to plot the Efficient Frontier, visually representing the optimal risk-return trade-off.

Optimal Portfolios: Identified both the Max Sharpe Ratio Portfolio and the Minimum Volatility Portfolio from the simulation.

Backtesting & Validation: Backtested the performance of the Max Sharpe Ratio portfolio against a simple equally-weighted portfolio and the S&P 500 (^GSPC) benchmark.

Key Findings from Backtesting
The backtesting results validated the effectiveness of the MPT-optimized portfolio. Over the backtesting period, the optimized portfolio demonstrated superior performance compared to both benchmarks:

Optimized Portfolio: 42% Cumulative Return

Equally-Weighted Portfolio: 40% Cumulative Return

S&P 500 Benchmark: 35% Cumulative Return

These results indicate that the optimization strategy successfully added value beyond a naive investment approach and the broader market. The project is now ready for final review and delivery.
**Task 4: Advanced Model Evaluation and Refinement**

This task focuses on a deeper analysis of the models and their outputs.

Model Comparison: A comparative analysis was performed to evaluate the predictive power of the ARIMA and LSTM models in detail, assessing their strengths and weaknesses.

Sensitivity Analysis: The sensitivity of the optimized portfolio to changes in key input parameters, such as the look-back period for returns or the risk-free rate, was examined.

Risk Metric Validation: The calculated VaR and other risk metrics were validated through historical backtesting to ensure they accurately reflect potential portfolio losses.

**Task 5: Final Report and Recommendations**

This final phase synthesizes all project findings into a comprehensive set of deliverables.
*
Report Generation: A detailed final report was compiled, summarizing the methodologies, key findings, and conclusions from each task.

Strategic Recommendations: Actionable investment recommendations were provided based on the portfolio optimization and backtesting results.

Future Work: A roadmap for potential future work, including the exploration of new models or the expansion of the portfolio, was outlined.