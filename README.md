# Whale Transfers & Price Movements Analysis

This project analyzes whether large whale transfers (>$100K) precede or correlate with significant price movements of a selected cryptocurrency token (e.g., ETH).

## Project Structure

- `test.ipynb`: Main analysis notebook. Fetches price and whale transfer data, preprocesses, merges, and visualizes relationships.
- `result.ipynb`: Contains summary insights and visualizations from the analysis.

## Workflow

1. **Select Token & Timeframe**
   - Choose a token (e.g., ETH)
   - Define a time range (e.g., last 30 days)

2. **Fetch Data**
   - Historical price data from CoinGecko API
   - Whale transfer data from Dune Analytics API

3. **Preprocess**
   - Convert timestamps to datetime
   - Resample/aggregate data to daily intervals

4. **Merge Datasets**
   - Join price and whale activity data on timestamp

5. **Analyze Correlation**
   - Calculate daily percent price change
   - Compute correlation between whale activity (amount, transactions, whales) and price movement

6. **Visualize**
   - Dual-axis line plots: price vs whale activity
   - Scatter plots: price change (%) vs whale metrics
   - Correlation matrix heatmap

## Key Insights

- **Whale transfer amount and price change** show a moderate negative correlation, suggesting large transfers may be linked to price drops.
- **Number of transactions and whales** are highly correlated, but both have weak relationships with price change.
- **Further analysis** (e.g., lagged effects, event studies) is recommended for deeper insights.
