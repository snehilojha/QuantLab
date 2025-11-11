# QuantLab

### Algorithmic Trading Strategy Backtesting Framework

**QuantLab** is a Python-based project for **backtesting and analyzing trading strategies** using historical market data.  
It helps traders, analysts, and researchers evaluate technical indicator-based strategies like **RSI**, **MACD**, **Bollinger Bands**, and **Moving Averages**.

---

## Features

- **Data Collection** — Automatically fetches OHLCV data via `yfinance`
- **Backtesting Engine** — Simulates trades using custom strategies
- **Technical Indicators** — Supports RSI, MACD, Bollinger Bands, SMA, EMA, and more
- **Performance Metrics** — Calculates cumulative returns, win rate, drawdown, and Sharpe ratio
- **Visual Analysis** — Interactive charts using `matplotlib` and `seaborn`
- **Extensible** — Add new strategies, indicators, or risk rules easily

---

## Key Modules
1. **Data Acquisition** -
  Fetches time-series price data for stocks, indices, or ETFs using yfinance.

2. **Data Cleaning & Preparation** -
  Handles missing values, computes log returns, and structures data for time-series analysis.

3. **Correlation & Covariance Analysis** -
  Calculates and visualizes correlation matrices and covariance heatmaps to study inter-asset relationships.

4. **Risk & Return Metrics** -
  Computes:
  Daily and cumulative returns
  Volatility
  Sharpe ratio and other performance indicators

5. **Visualization** -
  Generates:
  Time-series plots
  Pair plots and heatmaps
  Comparative performance charts

6. **Portfolio Evaluation (if included)** -
  Simulates simple or weighted portfolios to analyze expected returns and risk trade-offs.

---

## Installation & Setup

### Clone this Repository
``` bash
git clone https://github.com/snehilojha/QuantLab.git
cd QuantLab
pip install -r requirements.txt
```
### Or manually install required libraries
``` bash
pip install yfinance pandas numpy matplotlib seaborn
```

### Create a Virtual Environment
``` bash
python -m venv venv
source venv/bin/activate   # Mac/Linux
venv\Scripts\activate      # Windows
```

### Open the notebook in jupyter
``` bash
jupyter notebook QuantLab.ipynb
```
---

### Run cells sequentially to:

- Fetch financial data

- Perform analysis

- Visualize results

You can modify ticker symbols and time ranges to explore different assets or market periods.

---

## Example Outputs

- Correlation heatmaps between selected assets

- Time-series plots showing comparative returns

- Portfolio performance and risk metrics visualized
<img width="980" height="634" alt="output" src="https://github.com/user-attachments/assets/6dd6eca1-1a41-4c97-b1a1-3e329f65a8c9" />

- Above fig compares the return from SPY for last 20 years between (buy and hold) and trading using the simple moving average strategy.
