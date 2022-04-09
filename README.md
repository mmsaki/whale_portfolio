# 🐳 A Whale Portfolio analysis

# Table of Contents
1. Assignemnt background
2. Instructions
3. Results

## 🚧 1. Background

* Harold's company has been investing in algorithmic trading strategies. Some of the investment managers love them, some hate them, but they all think their way is best.

* You just learned these quantitative analysis techniques with Python and Pandas, so Harold has come to you with a challenge—to help him determine which portfolio is performing the best across multiple areas: volatility, returns, risk, and Sharpe ratios.

* You need to create a tool (an analysis notebook) that analyzes and visualizes the major metrics of the portfolios across all of these areas, and determine which portfolio outperformed the others. You will be given the historical daily returns of several portfolios: some from the firm's algorithmic portfolios, some that represent the portfolios of famous "whale" investors like Warren Buffett, and some from the big hedge and mutual funds. You will then use this analysis to create a custom portfolio of stocks and compare its performance to that of the other portfolios, as well as the larger market ([S&P 500 Index](https://en.wikipedia.org/wiki/S%26P/TSX_60)).

* For this homework assignment, you have three main tasks:
    * Read in and Wrangle Returns Data
    * Determine Success of Each Portfolio
    * Choose and Evaluate a Custom Portfolio

---

## 🚦	 2. Instructions

**File:** [Whale Analysis](/whale_portfolio/whale_analysis.ipynb)

* Whale Returns of Soros, Paulson,Tiger and Berkshire 
    * Read the Whale Portfolio daily returns and clean the data 
* Algorithmic 1 and Algorithmic 2 Daily Returns
    * Read the algorithmic daily returns and clean the data
* S&P 500 Returns
    * Read the S&P 500 historic closing prices and create a new daily returns DataFrame from the data.
* Combined Returns
    * Performance Anlysis
    * Calculate and Plot the daily returns.
    * Calculate and Plot cumulative returns.
    * Determine the risk of each portfolio:
        * Create a box plot for each portfolio.
        * Calculate the standard deviation for all portfolios
        * Determine which portfolios are riskier than the S&P 500
        * Calculate the Annualized Standard Deviation
    * Create a box plot for each portfolio
    * Calculate Standard Deviations
        * Determine which portfolios are riskier than the S&P 500
    * Calculate the Annualized Standard Deviation
    * Analyze the rolling statistics for Risk and Beta.
        * Calculate and plot the rolling standard deviation for all portfolios using a 21-day window
        * Calculate the correlation between each stock to determine which portfolios may mimick the S&P 500
        * Choose one portfolio, then calculate and plot the 60-day rolling beta between it and the S&P 500
    * Calculate and Plot Beta for a chosen portfolio and the S&P 500
        *  Try calculating the ewm with a 21-day half life for each portfolio, using standard deviation (std) as the metric of interest.
    * Using the daily returns, calculate and visualize the Sharpe ratios using a bar plot
        * Determine whether the algorithmic strategies outperform both the market (S&P 500) and the whales portfolios.
* Create Custom Portfolio
    * Choose 3-5 custom stocks with at last 1 year's worth of historic prices and create a DataFrame of the closing prices and dates for each stock.
        * Calculate the weighted returns for the portfolio assuming an equal number of shares for each stock
            * Join your portfolio returns to the DataFrame that contains all of the portfolio returns
        * Re-run the performance and risk analysis with your portfolio to see how it compares to the others
        * Include correlation analysis to determine which stocks (if any) are correlated
    * Calculate and Plot Rolling 60-day Beta for Your Portfolio compared to the S&P 500
    * Using the daily returns, calculate and visualize the Sharpe ratios using a bar plot
    * How does your portfolio do?
