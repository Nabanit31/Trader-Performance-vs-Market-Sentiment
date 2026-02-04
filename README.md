# Trader Performance vs Market Sentiment Analysis

## 📌 Project Overview
This project analyzes how **market sentiment (Fear, Greed, Neutral)** impacts **trader performance and behavior** using aggregated daily trader data aligned with a market sentiment index.  
The objective is to uncover behavioral patterns, performance differences, and actionable trading insights rather than build production-grade predictive models.

---

## 📂 Datasets Used
1. **Trader-level trading data**
   - Trade-level records aggregated into daily trader metrics
2. **Market sentiment data**
   - Daily Fear & Greed classification

---

## ⚙️ Data Preparation
- Converted timestamps to daily granularity
- Aggregated trade-level data to trader-day level
- Aligned trader metrics with daily sentiment
- Handled missing values and extreme ratios (`inf`) carefully
- Labeled missing sentiment as **Unknown** (used cautiously)

---

## 📊 Key Metrics Created
- Daily PnL per trader
- Win rate
- Average trade size
- Median trade size (leverage proxy)
- Trades per day
- Long/Short ratio
- PnL volatility

---

## 📈 Analysis Performed (Part B)

### Performance Analysis
- Average daily PnL by sentiment
- PnL distribution and volatility comparison
- Identification of risk-heavy regimes (Fear)

### Behavioral Analysis
- Trade frequency changes across sentiment regimes
- Leverage and position size variation
- Directional bias using long/short ratios (mean & median)

### Trader Segmentation
- High vs Low leverage traders
- Frequent vs Infrequent traders
- Consistent vs Inconsistent traders

---

## 🔍 Key Insights
- Fear regimes exhibit high volatility and extreme outcomes rather than consistent profitability
- Retail traders outperform during Greed and Extreme Greed regimes
- Whale traders generate higher average PnL during Fear but underperform during Greed
- Market sentiment affects extreme traders more than the median trader

---

## 🎯 Strategy Recommendations (Part C)
1. **During Fear regimes**, high-leverage and frequent traders should reduce position sizes and activity to limit drawdowns.
2. **During Greed regimes**, consistent traders can maintain trend-aligned strategies with controlled leverage.

---

## ⚠️ Limitations
- Limited overlap between sentiment and trader data reduces sample size
- Results are exploratory and behavior-focused
- Predictive modeling was explored but excluded due to data imbalance and reliability concerns

---

## ✅ Conclusion
This analysis demonstrates that market sentiment significantly influences trader behavior and performance, primarily by amplifying risk-taking among specific trader segments. The findings provide practical, data-driven guidance for adaptive trading strategies under different sentiment regimes.

---

## 🧑‍💻 Author
**Nabanit Roy**
