# Stock Support & Resistance Analysis with RSI

This Python project implements a stock analysis tool to calculate and visualize support and resistance levels for a given stock symbol. It also includes the calculation of the **Relative Strength Index (RSI)** to provide additional insights into the stock's price momentum.

The tool uses **yfinance** to fetch historical stock data, and **matplotlib** for plotting the results. The support and resistance levels are calculated by analyzing local minima and maxima over a specified lookback period. The RSI helps identify potential overbought or oversold conditions, providing signals for potential reversals or corrections.

## Features
- **Support and Resistance Levels**: Identifies potential price levels where the stock tends to reverse direction.
- **RSI Calculation**: Calculates the 14-day Relative Strength Index (RSI) to determine if the stock is overbought or oversold.
- **Interpretation**: Provides an interpretation of the latest price relative to the calculated support and resistance levels, as well as RSI.
- **Visualization**: Displays a plot of the stock's closing prices along with the calculated support and resistance levels.

## Requirements
Make sure to install the following libraries to run this project:

- `yfinance` – for fetching stock data
- `numpy` – for numerical operations
- `pandas` – for data manipulation
- `matplotlib` – for plotting

You can install the required dependencies using `pip`:

```bash
pip install yfinance numpy pandas matplotlib
```
## Usage

1. **Clone the repository** to your local machine:

   ```bash
   git clone https://github.com/your-username/stock-analysis-tool.git
   cd stock-analysis-tool
   ```
2. **Install the required dependencies** by running the following command:
   ```bash
   pip install -r requirements.txt
    ```
3. **Run the script by providing the stock symbol** (e.g., AAPL, TSLA, or Indian stock symbols with .NS suffix like RELIANCE.NS):
   ```bash
   python stock_analysis.py
    ```
4. **Example Usage**
   ```bash
   Enter any Ticker, For Indian Tickers Add Suffix wid .NS: NIFTYBEES.NS
     ```
5. **Example Output**
   ```bash
   --- Support & Resistance Summary ---
    Latest Close Price     : 150.25
    Latest Support Level   : 145.00
    Latest Resistance Level: 155.00
    Interpretation         : 🟢 Near Support (Potential Buying Opportunity)
    📢 Breakout Status      : ✅ Price is within Support & Resistance range (No breakout detected)
    
    --- RSI (14-day) Summary ---
    Latest RSI Value       : 72.35
    RSI Interpretation     : 🔴 RSI > 70 (Overbought — Possible correction)
    ```




