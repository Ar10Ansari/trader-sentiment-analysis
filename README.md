# 📊 Trader Performance vs Market Sentiment Analysis

## 📌 Objective

This project analyzes how Bitcoin market sentiment (Fear/Greed) influences trader behavior and performance on Hyperliquid. The goal is to uncover behavioral patterns and generate actionable strategy recommendations based on data-driven insights.

---

## 📂 Datasets Used

1. Bitcoin Fear & Greed Index  
   - Columns: Date, Classification (Fear, Extreme Fear, Greed, Extreme Greed, Neutral)

2. Hyperliquid Historical Trader Data  
   - Fields include: account, symbol, execution price, size, side, time, closedPnL, leverage, etc.

---

## ⚙️ Methodology

### 1️⃣ Data Preparation
- Loaded and validated both datasets
- Checked missing values and duplicates
- Converted timestamps to datetime
- Aggregated data at daily level
- Merged trader activity with sentiment classification

### 2️⃣ Feature Engineering
Constructed key analytical metrics:

- Daily PnL per trader
- Win rate (profitable trades / total trades)
- Trade frequency (daily trades)
- Average trade size
- Leverage distribution
- Long/Short ratio
- Volatility proxy (PnL standard deviation)

### 3️⃣ Trader Segmentation
Traders were segmented into behavioral archetypes:

- Aggressive Profitable (High risk, high return)
- Conservative Profitable (Low volatility, consistent returns)
- Underperforming (Inefficient risk-return profile)

---

## 📈 Key Insights

### 1️⃣ Fear Regimes Generate Higher Profitability
Average daily PnL peaks during Fear conditions, suggesting volatility-driven opportunities are better exploited during downturns compared to standard Greed periods.

### 2️⃣ Trade Size Expands During Fear
Average trade size increases significantly in Fear and Extreme Fear periods, indicating reactive or volatility-amplified behavior.

### 3️⃣ Two Distinct Profitable Archetypes Exist
Profitable traders cluster into:
- High-risk aggressive traders
- Low-volatility consistent traders  

Underperformers exhibit moderate volatility without proportional returns, indicating inefficient capital allocation.

---

## 🎯 Strategy Recommendations

### Strategy 1 – Volatility Exploitation Framework (Fear Regime)
- Allow increased exposure only for historically profitable traders
- Maintain strict stop-loss discipline
- Focus on structured volatility capture strategies

**Rationale:** Fear periods show highest average profitability.

---

### Strategy 2 – Overconfidence Control (Greed Regime)
- Cap leverage for high-frequency traders
- Normalize position sizing after consecutive wins
- Reduce trade frequency during prolonged Greed periods

**Rationale:** Greed regimes show lower profitability and potential overtrading bias.

---

## 🚀 How to Run

1. Clone repository:

# trader-sentiment-analysis

2. Install dependencies:


3. Open:


Run all cells sequentially.

---

## 📎 Repository Contents

- Structured Jupyter Notebook
- Sentiment vs Performance analysis
- Trader segmentation visualization
- Strategy recommendations
- Reproducible workflow
