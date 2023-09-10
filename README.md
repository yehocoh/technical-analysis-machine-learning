# technical-analysis-machine-learning
Predicting buy or sell orders using technical analysis and machine learning

## Project Name: Trading Strategy with Machine Learning

This repository contains a Python script for creating a trading strategy using machine learning. The script downloads historical stock price data for a list of symbols, applies technical analysis patterns, and uses a logistic regression model to make buy and sell predictions. The trading strategy is backtested on historical data, and portfolio performance metrics are calculated.

### Usage

To use this script, follow these steps:

1. Install the required Python packages by running the following commands:

   ```python
   %pip install vectorbt
   %pip install --upgrade urllib3
   %pip install yfinance
   %pip install TA-Lib
   ```

2. Open the script in a Python environment and execute it.

### Script Overview

The script performs the following steps:

1. Imports the necessary libraries, including `vectorbt`, `yfinance`, `talib`, and others.

2. Sets the number of days for historical data and a list of stock symbols to analyze.

3. Downloads historical stock price data for the specified symbols using Yahoo Finance.

4. Applies technical analysis patterns using the TA-Lib library.

5. Calculates the percentage change in stock prices.

6. Fits a logistic regression model to the technical analysis patterns to make buy and sell predictions.

7. Backtests the trading strategy by applying the predictions to the historical data.

8. Calculates portfolio performance metrics, including total return, volatility, drawdown, Sharpe ratio, and others.

### Example Output

Here is an example of the output produced by the script:

```python
Start                        2023-06-20 00:00:00
End                          2023-07-03 00:00:00
Period                          10 days 00:00:00
Total Return [%]                        1.702976
Benchmark Return [%]                    0.553845
Annualized Return [%]                1917.354302
Annualized Volatility [%]              24.217883
Max Drawdown [%]                        2.329061
Max Drawdown Duration            5 days 02:24:00
Sharpe Ratio                            1.987329
Calmar Ratio                       190305.231568
Omega Ratio                            74.932424
Sortino Ratio                         631.121227
Skew                                    0.626714
Kurtosis                                 1.72372
Tail Ratio                             56.290891
Common Sense Ratio                  10527.322183
Value at Risk                          -0.012738
Alpha                                   13.63703
Beta                                    0.644035
Name: agg_func_mean, dtype: object
```

### Note

This script is provided for educational and demonstration purposes only. The trading strategy and performance metrics are based on historical data and may not be suitable for actual trading. Use it at your own risk.

For any questions or issues, please feel free to create an issue in this GitHub repository.

Happy trading!
