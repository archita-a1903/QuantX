# ⚡ QuantX — Multi-Asset Portfolio Backtesting & Trading Strategy Simulator

QuantX is an advanced **Streamlit-based quantitative trading research toolkit** that lets you design, test, and visualize trading strategies with just a few clicks.  
It combines **technical indicators**, **multiple trading strategies**, and a **vectorized multi-asset backtesting engine** giving you powerful analytics, portfolio performance metrics, and visual insights in real-time.

> ⚠️ For research and educational use only. QuantX does **not** provide financial or investment advice.

---

## 🚀 Features

- 🧠 **Interactive Dashboard (Streamlit UI)** — Run backtests, visualize charts, and export reports instantly.  
- 📈 **Technical Indicators Included**
  - Exponential Moving Averages (EMA)
  - Relative Strength Index (RSI)
  - MACD (line, signal, histogram)
  - Bollinger Bands
  - Average True Range (ATR)
  - Rolling Volatility
- 🧩 **Built-in Trading Strategies**
  - **EMA + RSI + Volatility Filter** — Trend following with risk gating  
  - **Bollinger Mean Reversion** — Buy dips, sell rallies  
  - **MACD Trend Following** — Signal crossover-based trend capture
- 💰 **Portfolio Backtesting Engine**
  - Multi-asset allocation with cash accounting  
  - Slippage and commission modeling  
  - Performance metrics: Total Return, Annualized Return, Volatility, Sharpe Ratio, Max Drawdown  
- 📊 **Visual Analytics & Export**
  - Equity curve plots, asset-level risk/return charts, trade logs  
  - One-click Excel export for all trades and portfolio results

---

## 🧩 File Overview

| File | Description |
|------|--------------|
| `app.py` | Streamlit dashboard UI, plots, metrics, and Excel export |
| `backtester.py` | Core backtesting engine handling trades, positions, and performance |
| `data.py` | Market data ingestion using Yahoo Finance (`yfinance`) |
| `features.py` | Implements EMA, RSI, MACD, Bollinger Bands, ATR, and volatility |
| `strategies.py` | Defines multiple strategy logics built on the indicators |
| `requirements.txt` | Python dependencies for the environment |

---

## ⚙️ Installation & Setup

```bash
# 1️⃣ (Optional) Create a virtual environment
python -m venv .venv
source .venv/bin/activate   # macOS / Linux
# .venv\Scripts\activate    # Windows

# 2️⃣ Install dependencies
pip install -r requirements.txt

# 3️⃣ Launch the dashboard
streamlit run app.py

 🧠 Usage
1. Select tickers (e.g. AAPL, MSFT, JPM)
2. Choose your backtest date range and trading strategy
3. Adjust indicator parameters (EMA, RSI, etc.)
4. Click Run Backtest
5. View performance charts, metrics, and per-asset results
6. Export your results as an Excel report

📊 Key Performance Metrics
1. Total Return (%)
2. Annualized Volatility
3. Sharpe Ratio
4. Maximum Drawdown
5. Number of Trades
6. Profit Factor

🧰 Technologies Used
1. Python 3.10+
2. Streamlit
3. pandas
4. numpy
5. matplotlib
6. plotly
7. yfinance
8. scipy
