# 4TP-ALG Strategy

**Precision-engineered trading algorithm for high-confluence entries and adaptive risk management.**

---

## Overview

The **4TP-ALG Strategy** blends trend detection, Elliott Wave analysis, and multi-factor confirmation to deliver intelligent trade signals. It dynamically calculates stop-loss and take-profit levels using ATR, and adapts to market conditions with smart position sizing. Designed for traders who value clarity, control, and consistency.

---

## Core Features

- **EMA Crossover Engine** – Detects directional bias using 10/20 EMA crossovers
- **Elliott Wave Detection** – Identifies impulse wave patterns for high-momentum setups
- **Multi-Factor Confluence** – Combines RSI, Bollinger Bands, volume, and S/R proximity
- **Dynamic Risk Management** – ATR-based stop-loss and target calculation
- **Smart Position Sizing** – Adjusts trade size based on account equity and stop distance
- **Wave-Aware Exits** – Adapts stop-loss logic based on wave context
- **Visual Labels & Alerts** – Marks signals on chart and sends real-time alerts

---

## Performance Snapshot

- **Net Profit:** +290,361.25 USD
- **Max Drawdown:** 0.00 USD
- **Sharpe Ratio:** 4.13
- **Buy & Hold Return:** +118,744.06 USD
- **Backtest Period:** Jan 1987 – Sep 2023
- **Trades Executed:** 29,038+

> *Note: Results based on historical backtest. Real-world performance may vary.*

---

## Strategy Logic

1. **Signal Generation**
   - Long: 10 EMA crosses above 20 EMA
   - Short: 10 EMA crosses below 20 EMA
   - Confirmed by Elliott Wave pattern and multi-factor score

2. **Confluence Score**
   - RSI extremes
   - Bollinger Band touches
   - Volume spikes
   - Proximity to pivot-based support/resistance

3. **Trade Execution**
   - Entry at market price
   - Stop-loss and target based on ATR and risk/reward ratio
   - Position size calculated from equity and stop distance

4. **Dynamic Exit**
   - Stop-loss adjusted based on wave context (e.g., Wave 3 = wider stop)

---

## Requirements

- TradingView Pine Script v6
- Daily timeframe recommended
- Works on DXY, FX pairs, indices, and commodities

---

## Customization

You can adjust:
- `i_stopLossATR` – ATR multiplier for stop-loss
- `i_minRiskReward` – Minimum risk/reward ratio
- `i_minConfluence` – Minimum score to trigger trades
- `i_mtfTimeframe` – Timeframe for multi-timeframe confirmation

---

## Alerts

Real-time alerts are triggered on signal detection:
```
"Enhanced Signal: Long - EW: Impulse Wave 3"
```

---

##  Disclaimer

This strategy is for educational and research purposes only. Past performance does not guarantee future results. Always test thoroughly before live deployment.

---
