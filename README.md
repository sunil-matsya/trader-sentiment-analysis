# Trader Performance vs Market Sentiment Analysis

## Problem Statement
This project analyzes the relationship between Bitcoin market sentiment (Fear vs Greed)
and trader performance using historical trading data from Hyperliquid.

## Datasets Used
1. Bitcoin Market Sentiment Dataset  
   - Columns: Date, Classification (Fear / Greed)

2. Historical Trader Data (Hyperliquid)  
   - Columns include Account, Side, Trade Size (USD), Timestamp, Closed PnL, etc.

## Methodology
- Cleaned and standardized date formats
- Merged trader data with daily market sentiment
- Analyzed performance metrics such as profit/loss and win rate
- Studied behavioral patterns like trade size, trade count, and buy/sell bias
- Visualized findings using clear, interpretable charts

## Key Insights
- Trading activity and trade sizes are higher during Greed periods
- Greed phases show higher volatility in profit and loss
- Fear periods encourage more conservative trading behavior
- Higher confidence does not always translate into higher win rates

## Conclusion
Market sentiment strongly influences trader behavior and risk-taking.
Sentiment can be used as a risk-management signal rather than a profit guarantee.

## Tools Used
- Python
- Pandas
- Matplotlib
- Seaborn
