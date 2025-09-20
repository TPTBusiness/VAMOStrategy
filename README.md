# VAMOStrategy

**VAMOStrategy** — an open-source Pine Script v6 trading *strategy* for TradingView, built for Bitcoin scalping.

The VAMO Crossover Strategy uses a Volatility-Adjusted Momentum Oscillator (VAMO) and an EMA signal line to generate buy/sell signals. It adds ATR-based stop loss / take profit and a volatility filter for cleaner, faster scalping decisions.

---

## Features

- **VAMO indicator** — combines momentum (ROC) and volatility (ATR) for adaptive signals.  
- **Crossover signals** — long/short entries triggered when VAMO crosses its EMA signal line.  
- **Risk management** — ATR-based stop (default 1× ATR) and take-profit (default 2× ATR).  
- **Volatility filter** — skips trades in high-volatility regimes to reduce false signals.  
- **Customizable** — tweak periods, stop/take multipliers and filters to fit your style.

---

## Quick setup

1. Open **TradingView** and go to the **Pine Editor**.  
2. Copy the code from `Strategy.pine` in this repository.  
3. Paste it into the Pine Editor and click **Add to Chart**.  
4. Apply to a Bitcoin chart (e.g. `BTC/USD` or `BTC/USDT`) on a **1–5 minute** timeframe.  
5. Open the strategy settings and adjust inputs (Momentum Length, Volatility Length, Signal Length, Take Profit Multiplier, etc.).

**Recommended starting inputs (example)**  
- Momentum Length: `5`  
- Volatility Length: `5`  
- Signal (EMA) Length: `3`  
- Stop Loss: `1 × ATR`  
- Take Profit: `2 × ATR`

---

## Scalping tips

- **Timeframe:** 1–5 minute charts are recommended for Bitcoin scalping.  
- **Optimize inputs:** try faster settings for quicker signals (see recommended inputs above).  
- **Backtest:** run thorough backtests on historical BTC data to refine parameters.  
- **Leverage:** if you choose to use leverage, consider 5–20× and manage position size and risk carefully.  
- **Paper trade first:** always test on a demo account before trading real funds.

---

## Contributing

We welcome contributions! Ways to help:

- Propose new indicators, filters (e.g., volume-based), or exit rules.  
- Optimize parameters for different assets or timeframes.  
- Fix bugs or improve code readability and performance.  
- **How to contribute:** fork the repo, make your changes, and submit a pull request. Use the Issues tab to discuss ideas.

> Contributing Guide: *coming soon*

---

## Repository structure

- `Strategy.pine` — VAMO Crossover Strategy (Pine Script v6).  
- `LICENSE` — MIT License.  
- `README.md` — this file.

---

## License

Licensed under the **MIT License**. See the `LICENSE` file for details.  
© 2025 TPTBusiness

---

## Disclaimer

This strategy is provided **"as is"** without warranty. Trading carries high risk and past performance is not indicative of future results. Test thoroughly and understand the code before using real funds. This repository is educational — nothing here is financial advice.

