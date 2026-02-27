# BTC Momentum EMA-RSI Backtest

Production-grade backtesting and optimization engine for a BTC-USD momentum strategy using EMA crossovers and RSI filters with in-sample/out-of-sample validation.

---

## Strategy Logic

- Long-only momentum system
- Entry:
  - EMA(short) crosses above EMA(long)
  - RSI > threshold
- Exit:
  - EMA(short) crosses below EMA(long)
  - OR RSI < threshold

---

## Features

- Vectorized backtesting engine
- Parameter grid search (two-stage optimization)
- In-sample / Out-of-sample validation
- Performance metrics:
  - CAGR
  - Sharpe Ratio
  - Max Drawdown
  - Win Rate
  - Profit Factor
  - Consecutive Losses
- Equity & Drawdown visualization
- PDF export support

---

## Data

- Source: Yahoo Finance
- Asset: BTC-USD
- Timeframe: Daily
- Period: Jan 2020 – Jan 2024

---

## Installation

```bash
pip install -r requirements.txt
