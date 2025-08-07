# Whale Transfers & Price Movements Analysis

Analyze whether large whale transfers (>$100K) precede or correlate with significant price movements of a selected cryptocurrency token.

## Project Structure

- `test.ipynb`: Main analysis notebook.
- `result.ipynb`: Summary insights and visualizations.

## Setup

1. **Clone the repository**
   ```sh
   git clone https://github.com/yourusername/Large-ETH-Transfers-vs-Price.git
   cd Large-ETH-Transfers-vs-Price
   ```

2. **Install dependencies**
   ```sh
   pip install pandas requests matplotlib seaborn scipy python-dotenv
   ```

3. **Configure API keys**
   - Create a `.env` file in the project root:
     ```
     DUNE_API=your_dune_api_key_here
     GECKO_API=your_coingecko_api_key_here
     ```
   - If you don’t have API keys,
   - Sign up on Dune, go to settings > API. Generate and copy your API Key
   - Sign up for a CoinGecko API Account. Generate and copy your API Key
4. **Run the notebook**
   - Open `test.ipynb` in Jupyter or VS Code.
   - Run all cells to reproduce the analysis.

## Resources

- [CoinGecko API](https://docs.coingecko.com/v3.0.1/reference/setting-up-your-api-key)
- [Dune Analytics API](https://docs.dune.com/api-reference/overview/introduction)
- Dune Query:  
  [Whale Transfers Query](https://dune.com/queries/5591956)

## Workflow

1. Fetch price and whale transfer data via APIs.
2. Preprocess and aggregate data.
3. Merge datasets on timestamp.
4. Analyze correlations and visualize results.

## Key Insights

- Whale transfer amount shows a moderate negative correlation with price change.
- Number of transactions and whales are highly correlated, but weakly related to price change.
- Further analysis recommended for deeper insights.
  
*For research and educational purposes only.*
