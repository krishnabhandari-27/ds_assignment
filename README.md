# Trader Performance vs Market Sentiment Analysis

## Overview

This project analyzes the relationship between Bitcoin market sentiment (Fear/Greed Index) and trader behavior on Hyperliquid.  
The objective is to evaluate how sentiment impacts trading performance, activity levels, risk-taking behavior, and directional bias, and to derive actionable strategy insights.

---

## Dataset Description

Two datasets were used:

1. **Bitcoin Market Sentiment Dataset**
   - Date
   - Sentiment Classification (Fear, Greed, Extreme Fear, Extreme Greed, Neutral)

2. **Historical Trader Execution Dataset**
   - Account
   - Execution Price
   - Size USD
   - Direction (Open Long / Open Short)
   - Closed PnL
   - Timestamp

---

## Methodology

### 1. Data Preparation
- Loaded both datasets.
- Converted timestamps to daily format.
- Merged trader data with sentiment data on date.
- Checked for missing values and duplicates.

### 2. Feature Engineering
Created key metrics:
- Daily total PnL
- Win rate
- Trade frequency per day
- Average trade size
- Long/Short ratio
- Trader segmentation:
  - Frequent vs Infrequent traders
  - Consistent winners vs Inconsistent traders

### 3. Analysis
- Compared performance across Fear vs Greed regimes.
- Evaluated changes in trade frequency and trade size.
- Analyzed directional bias using Long/Short ratio.
- Compared behavior across trader segments.

---

## Key Insights

### 1. Performance is Higher During Fear Periods
Average daily PnL is significantly higher during Fear and Extreme Fear regimes compared to Greed periods. However, risk and price swings are also higher during Fear days.

### 2. Traders Become More Active During Fear
Trade frequency increases sharply during Fear regimes, indicating stronger participation during uncertain or volatile market conditions.

### 3. Directional Bias Shifts with Sentiment
Traders take more long positions during Fear and relatively more short positions during Greed, suggesting sentiment-driven positioning behavior.

---

## Strategy Recommendations

### Strategy 1: Risk-Adjusted Trading During Fear
Increase participation during Fear regimes but reduce position size to manage elevated downside risk.

### Strategy 2: Sentiment-Based Directional Bias
Favor long setups during Fear regimes and reduce long exposure or consider short positions during Greed regimes.

---

