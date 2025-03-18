## Project Summary  

This project simulates an algorithmic trading scenario, assuming access to historical NYSE stock market data dating back to 1960. The goal was to strategically create sequences of stock buy-and-sell orders, maximizing profits under realistic constraints, including:

- **Initial Investment**: Starting from $1.
- **Transaction Limits**: Each daily trade limited to a maximum of 10% of the stock's daily traded volume.
- **Commission Costs**: 1% commission applied per transaction (buying or selling).
- **Trade Timing**: Trades categorized by market timing:
  - Opening (buy/sell at open price)
  - Intraday (buy at daily low, sell at daily high)
  - Closing (buy/sell at closing price)

Two trading sequences were generated:

- **`small.txt`**: Optimized sequence (≤1000 transactions).
- **`large.txt`**: Extensive high-profit sequence (≤1,000,000 transactions).

Methods included heuristic-driven trade selection, thorough data preprocessing, and valuation tracking over time.

Results were documented with profitability graphs and detailed explanations in the accompanying `report.pdf`. Code is also provided in the corresponding ipynb file. 

**Note:** This project was conducted as part of an academic assignment.
