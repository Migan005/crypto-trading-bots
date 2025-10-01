# Crypto Trading Bots

This repository contains automated trading bots for Bybit futures, built with Freqtrade and Python. Designed for traders seeking profitable, automated strategies.

## Professional Bybit Strategy
- **File:** `professional_bybit_strategy.py`
- **Description:** A trading bot for Bybit futures (BTC/USDT, ETH/USDT, 5m timeframe). Uses RSI, MACD, and ATR indicators with dynamic leverage (2–3x) and custom stoploss logic. Backtested to achieve 10%+ ROI over 60 days.
- **Features:**
  - RSI (<30 buy, >70 sell), MACD crossover, ATR volatility filter.
  - 1h timeframe RSI for trend confirmation.
  - Dynamic leverage adjustment based on market volatility.
  - Trailing stoploss to protect profits.
- **Usage:**
  1. Install Freqtrade: `pip install freqtrade`
  2. Configure Bybit API in `config.json` (see [Freqtrade docs](https://www.freqtrade.io)).
  3. Run backtest: `freqtrade backtesting --strategy ProfessionalBybitStrategy`
  4. Run live: `freqtrade trade --strategy ProfessionalBybitStrategy`

## Setup
- **Requirements:** Python 3.12+, Freqtrade, pandas_ta, ccxt.
- **Testing:** Always test in dry-run mode first (`--dry-run`).

## License
MIT License. Free to use and modify.

## Contact
Available for custom bot development on Upwork: https://www.upwork.com/freelancers/~0119bb7510534853df?mp_source=share
