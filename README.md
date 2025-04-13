# Bollinger Bands & MACD-Based Equity Trading Strategy

This project develops a hybrid quantitative trading strategy combining **Bollinger Bands** and **MACD** indicators to model volatility, detect anomalies, and generate actionable trading signals from stock market data.

---

## Objective

To implement a rule-based equity trading strategy using real-time price data, focused on:
- Identifying statistically significant price deviations using Bollinger Bands
- Capturing trend shifts using MACD (Moving Average Convergence Divergence)
- Evaluating the strategy’s risk-adjusted performance via Sharpe Ratio and signal precision

---

## Methodology

### Data Source
- Real-time equity data fetched via **Quandl API**
- Daily historical stock prices

### Indicators Used
- **Bollinger Bands**: 20-day SMA ± 2×std deviation (volatility detection)
- **MACD**: (12-day EMA − 26-day EMA), with 9-day signal line (momentum detection)

### Trading Logic
| Condition | Trigger |
|----------|---------|
| **Buy**  | Price crosses below lower Bollinger Band AND MACD shows bullish crossover |
| **Sell** | Price crosses above upper Bollinger Band AND MACD shows bearish crossover |

---

## Results

| Metric | Value |
|--------|-------|
| Anomaly Detection Accuracy | **93%** |
| Trend Forecasting Precision | **90%** |
| Sharpe Ratio | **0.047** |

The strategy exhibits strong alignment between signal triggers and market movement, resulting in a high signal-to-noise ratio and promising profitability potential.

---

## Key Highlights
- Fully implemented in **Python** using **Pandas**, **Matplotlib**, and **Plotly**
- Visualization of bands, signals, and equity price in interactive and static formats
- Performance metrics calculated directly from return series
- Modular code structure for easy extension and backtesting

---

## Future Improvements
- Add win rate and drawdown analysis
- Extend to multiple equities and cross-validation
- Incorporate slippage and transaction cost models
- Tune indicator parameters with grid search

---

## Author

**Saksham Gupta**  
Final Year, B.S. in Mathematics and Computing  
Indian Institute of Technology, Kharagpur  
Email: gsaksham.iitkgp@gmail.com  
[LinkedIn](https://www.linkedin.com/in/saksham-gupta23) • [GitHub](https://github.com/saksham-gupta23)

---
