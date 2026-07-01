# Trader Performance vs. Bitcoin Market Sentiment

Analysis of how trader behavior and performance on Hyperliquid relate to Bitcoin market sentiment (Fear/Greed Index).

## Datasets
- **Fear/Greed Index** — daily BTC sentiment classification (Extreme Fear → Extreme Greed)
- **Hyperliquid Historical Data** — trade-level data (account, coin, price, size, side, closed PnL, etc.)

## How to Run
Open `khanak.ipynb` in Google Colab → Runtime → Run all.
The first cell auto-downloads both CSVs from Google Drive — no manual upload needed.

## What's Inside
1. Data loading & cleaning
2. Merging trades with daily sentiment
3. PnL & win rate by sentiment regime
4. Trading activity & position sizing by sentiment
5. Long/short positioning by sentiment
6. PnL distribution & time series vs. sentiment
7. Per-account performance breakdown
8. Exposure/sizing analysis
9. Key findings & strategy implications

## Key Findings
1. **PnL & win rate** are highest in Extreme Greed, weakest in Extreme Fear/Neutral.
2. **Activity & trade size peak during Fear** (not the extremes) — traders are most active and heavily positioned in moderate fear.
3. **Positioning is contrarian**, not trend-following — traders go net long during Fear and net short during Greed.
4. **Performance varies by account** — most top accounts are profitable only in specific regimes; one account stays consistently profitable across nearly all of them, suggesting real skill.
5. **Position sizing (relative to existing exposure) drops at sentiment extremes** — traders scale back at Extreme Fear and Extreme Greed alike.

## Strategy Implications
- Favor contrarian entries during Fear, where positioning is already profitable.
- Reduce size at sentiment extremes, mirroring how traders already behave.
- Prioritize capital allocation toward accounts with cross-regime consistency over those that only spike in favorable sentiment.
