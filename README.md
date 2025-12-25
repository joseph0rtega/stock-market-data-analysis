# Stock Market Data Analysis & Insights (2019–2024)

Data analysis project that explores historical stock behavior using real market data from Yahoo Finance.
Instead of predicting prices, the goal is to extract **clear insights** from returns, volatility, drawdowns, volume spikes, and correlations.

## What this project does
- Downloads daily historical stock data (default tickers: AAPL, MSFT, NVDA, SPY)
- Cleans and reshapes the dataset into a tidy format (`date`, `ticker`, `close`, `volume`)
- Computes key analytics:
  - daily returns
  - annualized volatility
  - drawdown and maximum drawdown
  - volume spike detection (top 10% volume days per ticker)
  - next-day return comparison (spike vs normal days)
  - return correlation matrix
- Produces charts + written insights in a notebook

## Key insights (high level)
- NVDA showed the strongest growth but also the highest risk (volatility) and deepest max drawdown.
- SPY was the most stable, reflecting the benefits of diversification.
- Volume spikes were followed by different next-day return behavior depending on the asset (e.g., NVDA differed from AAPL/MSFT/SPY).
- Correlation analysis showed moderate positive correlation between SPY and large-cap tech, with lower pairwise correlations across individual stocks.

## Tech stack
- Python
- pandas, NumPy
- matplotlib
- yfinance
- (Notebook built and run in Google Colab)

## How to run (local)
1) Install dependencies:
```bash
pip install -r requirements.txt
