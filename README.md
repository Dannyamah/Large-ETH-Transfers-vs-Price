# Whale Transfers & Price Movements Analysis

This project analyzes whether large whale transfers (>$100K) precede or correlate with significant price movements of a selected cryptocurrency token (e.g., ETH).

## Project Structure

- `test.ipynb`: Main analysis notebook. Fetches price and whale transfer data, preprocesses, merges, and visualizes relationships.
- `result.ipynb`: Contains summary insights and visualizations from the analysis.

## Key Insights

- **Whale transfer amount and price change** show a moderate negative correlation, suggesting large transfers may be linked to price drops.
- **Number of transactions and whales** are highly correlated, but both have weak relationships with price change.
- **Further analysis** (e.g., lagged effects, event studies) is recommended for deeper insights.
