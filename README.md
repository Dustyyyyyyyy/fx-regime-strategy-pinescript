# FX Regime Strategy (TradingView / Pine Script)

This repo contains a TradingView Pine Script strategy built to study market regimes using:
- EMA slope (trend direction/strength proxy)
- ATR + normalized volatility
- normalized volume
- RSI + ADX filters

## What’s inside
- `strategy.pine` – full strategy code
- `results/` – screenshots of Strategy Tester metrics

## Backtest snapshot (example)
Instrument: AUDUSD
Timeframe: 1 hour  
Period: Jan 2025 – Jan 2026  
Position sizing: 0.25 lots (fixed)  
Costs modeled: commission + slippage (see Pine `strategy()` settings)

Key metrics (TradingView Strategy Tester):
- Net return: +18.85%
- Max drawdown: 2.16%
- Trades: 85
- Win rate: 47.1%
- Profit factor: 1.96

## Notes / Assumptions
- Backtests are for research/learning purposes; results may vary live due to spread, slippage, and broker execution.
- Strategy uses end-of-bar execution (`process_orders_on_close`).

## How to run
1. Open TradingView → Pine Editor
2. Paste code from TradingView Pinecode
3. Add to chart and review Strategy Tester
