Overview
This project explores the relationship between Bitcoin market sentiment (Fear & Greed Index) and trader performance using historical trading data from Hyperliquid.
The analysis uncovers hidden patterns in profitability, trading volume, and trade behavior under different sentiment conditions, providing insights that can drive smarter trading strategies.

-Datasets

Historical Trader Data (Hyperliquid)
Columns: account, symbol, execution price, size, side, time, start position, Closed PnL, leverage, etc.
Fear & Greed Index (Bitcoin Sentiment)
Columns: date, classification (Fear / Greed).
Both datasets are merged on the date column, aligning trades with market sentiment for that day.

-Workflow

Data Loading & Preprocessing
Read historical trader data and sentiment index from CSV files.
Convert timestamps to consistent date formats.
Merge datasets on date.
Analysis Performed
Average Closed PnL by sentiment.
Total Trading Volume (USD) by sentiment.
Trade Side Distribution (Buy vs. Sell) across sentiments.
Profitability comparison of Buy vs. Sell trades in Fear vs. Greed.

-Visualizations
Bar charts and stacked bar plots for PnL, volume, and trade distribution.
All plots are saved as .png files.

-Output

Merged dataset exported as merged_trader_sentiment_data.csv.
Insights visualized and saved locally

-Sample Insights
Traders may achieve higher profitability during Greed phases, reflecting stronger risk-taking behavior.
Trading volume often spikes during Fear, suggesting higher uncertainty-driven activity.
Buy vs. Sell performance highlights which strategy works best under different sentiment conditions.

-Visualizations

pnl_by_sentiment.png
volume_by_sentiment.png
side_by_sentiment.png
pnl_by_side_sentiment.png
