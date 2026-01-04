# Trader Performance vs Market Sentiment Analysis

## Assignment Overview
This project explores the relationship between **Bitcoin market sentiment** and **trader performance and behavior** using historical trading data from Hyperliquid.  
The goal is to uncover how market emotions such as Fear and Greed influence profitability, risk-taking, and participation, and to derive insights that can support **smarter trading strategies**.

---

## Datasets Used

### 1. Bitcoin Market Sentiment Dataset
- Columns:
  - `date`
  - `classification` (Extreme Fear, Fear, Neutral, Greed, Extreme Greed)
- Represents daily market sentiment for Bitcoin.

### 2. Historical Trader Data (Hyperliquid)
- Columns include:
  - `Account`
  - `Coin`
  - `Side` (BUY / SELL)
  - `Size USD`
  - `Timestamp IST`
  - `Closed PnL`
- Represents execution-level historical trading activity.

---

## Data Source
The datasets were provided as part of the assignment:

- **Historical Trader Data**  
  https://drive.google.com/file/d/1IAfLZwu6rJzyWKgBToqwSmmVYU6VbjVs/view

- **Bitcoin Fear & Greed Index**  
  https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc_-mnrYv_nhSf/view

The datasets are included in this repository for reproducibility.

---

## Methodology
1. Converted timestamps and standardized date formats.
2. Extracted trade-level dates from intraday timestamps.
3. Merged trader data with daily market sentiment using the date as a common key.
4. Computed performance metrics such as average profit/loss, median profit/loss, and win rate.
5. Analyzed behavioral patterns including trade count, trade size, and buy/sell distribution.
6. Visualized results using clear and interpretable charts.

---

## Quantitative Summary

### Performance Summary
- **Extreme Greed** shows the highest average profitability and win rate.
- Median profit/loss is zero across all sentiment categories, indicating that most trades close near break-even.
- Win rates remain below 50% even in favorable conditions, suggesting profitability depends on payoff size rather than frequent wins.

### Behavior Summary
- Trading activity is highest during **Fear** and **Greed** periods.
- **Fear periods show the largest average trade sizes**, indicating fewer but higher-conviction trades.
- **Extreme Greed exhibits smaller average trade sizes** despite higher participation.
- Buy vs Sell ratios are relatively balanced, with a slight selling bias during Greed phases.

---

## Visual Analysis & Interpretation

### Trader PnL Distribution under Fear vs Greed
The PnL distribution shows higher volatility during Greed and Extreme Greed periods, with both large gains and large losses. Fear and Extreme Fear periods display more compact distributions, indicating more controlled outcomes. Median PnL remains near zero across all sentiment categories.

### Average Trade Size by Market Sentiment
Average trade size is highest during Fear and lowest during Extreme Greed. This suggests that traders take larger positions when sentiment is fearful, while euphoric periods attract more participants trading smaller positions.

### Number of Trades by Market Sentiment
Trade counts peak during Fear and Greed phases, while Extreme Fear has the lowest participation. This highlights how sentiment influences trader engagement and opportunity perception.

### Win Rate by Market Sentiment
Extreme Greed shows the highest win rate, followed by Fear. However, win rates remain below 50% across all categories, reinforcing that effective trading relies on risk management rather than sentiment alone.

---

## Key Insights
- Market sentiment strongly influences trader participation and risk-taking behavior.
- Greed increases activity and volatility but does not guarantee consistent profitability.
- Fear encourages fewer but larger trades, indicating selective risk exposure.
- Profitability is driven by a small number of high-impact trades rather than frequent wins.
- Sentiment is best used as a **risk-management indicator**, not a direct profit signal.

---

## Conclusion
This analysis demonstrates that Bitcoin market sentiment affects not only trader performance but also how traders participate and size their positions. While optimistic sentiment increases engagement and volatility, it does not ensure higher success rates. Incorporating sentiment awareness can help traders manage risk more effectively and make more informed decisions.

---

## Tools Used
- Python
- Pandas
- Matplotlib
- Seaborn
