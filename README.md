## Setup
pip install pandas numpy matplotlib seaborn scikit-learn

## How to Run
1. Place sentiment.csv and trades.csv inside data/ folder
2. Open notebook.ipynb in Jupyter
3. Run all cells top to bottom

## Methodology
- Loaded Hyperliquid trade data and Bitcoin Fear/Greed index
- Parsed timestamps, aligned both datasets on daily date
- Computed daily per-trader metrics: PnL, win rate, trade count, position size, long ratio
- Segmented traders by frequency, consistency, and total PnL
- Compared all metrics across Fear vs Greed sentiment days
- Built a Random Forest model to predict next-day profitability

## Key Insights
1. Win rate is higher on Greed days - traders perform better when sentiment is positive
2. Frequent traders outperform on Greed days but suffer more on Fear days due to overtrading
3. Consistent winners use smaller position sizes and maintain steadier PnL

## Strategy Recommendations
1. Fear days: Reduce position size by 30-40%, avoid new longs, prefer short or neutral
2. Greed days: Active traders can increase frequency; passive traders wait for clear setups

## Files
- notebook.ipynb - full analysis
- charts/ - all saved charts
- data/ - input datasets

