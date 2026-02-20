# 📊 Amazon Stock Market Analysis Dashboard  
### A Comprehensive Financial Data Analysis & Excel Dashboard Project

> An end-to-end financial data analysis project exploring Amazon’s historical stock performance (1997–Present), featuring data cleaning, feature engineering, trend classification, pivot modeling, and interactive dashboard development using Microsoft Excel.

---

## 📌 Executive Summary  

This project analyzes over **7,000+ trading days** of Amazon stock data to identify patterns in:

- Market direction (Bullish, Bearish, Neutral)
- Trading volume behavior
- Trend confirmation strength
- Price volatility dynamics
- Momentum signals

Using Excel as a full analytical environment, I transformed raw financial data into structured insights through calculated metrics, pivot modeling, and an interactive dashboard designed for decision support.

The final output is a professional dashboard capable of revealing volume trends, price behavior, and directional market consistency over time.

---

# 🎯 Business Problem  

Financial markets generate massive volumes of time-series data. However, raw stock data alone does not provide actionable insight.

Key analytical questions addressed in this project:

- How often does Amazon trade in bullish vs bearish conditions?
- Does trading volume support price direction?
- Are confirmed trends more stable than unconfirmed ones?
- How does price volatility behave across trend types?
- Can volume shifts signal momentum changes?

This project answers those questions using structured financial analysis techniques.

---

# 🗂️ Dataset Overview  

**Dataset:** Historical Amazon Stock Data  
**Time Period:** 1997 – Recent Years  
**Observations:** 7,086 Trading Days  
**Granularity:** Daily  

### 📑 Raw Dataset Structure  

| Column | Description |
|--------|------------|
| Date | Trading date |
| Open | Opening price |
| High | Highest price of the day |
| Low | Lowest price of the day |
| Close | Closing price |
| Volume | Number of shares traded |
| Price Range | Daily volatility (High − Low) |
| Market Movements | Bullish / Bearish / Neutral |
| Volume Level | Increasing / Decreasing |
| Trends | Confirmed Uptrend / Confirmed Downtrend / Unconfirmed |

---

# 🛠️ Data Preparation & Transformation  

## 1️⃣ Data Cleaning  

- Standardized date formats  
- Validated numeric data types  
- Removed inconsistencies  
- Verified chronological order  
- Ensured no structural breaks in time series  

---

## 2️⃣ Feature Engineering  

### 🔹 Price Range (Volatility Proxy)

```excel
=High - Low
```

Used as a measure of daily volatility.

---

### 🔹 Market Movement Classification  

Logic:

- **Bullish** → Close > Open  
- **Bearish** → Close < Open  
- **Neutral** → Close = Open  

This converts raw price data into directional market behavior.

---

### 🔹 Volume Level Classification  

```excel
=IF(Current Volume > Previous Day Volume, "Increasing", "Decreasing")
```

This helps determine whether momentum is strengthening or weakening.

---

### 🔹 Trend Identification  

Based on directional consistency:

- Confirmed Uptrend  
- Confirmed Downtrend  
- Unconfirmed Trend  

This classification improves reliability of directional analysis.

---

# 📊 Pivot Modeling Strategy  

Pivot tables were created to:

- Aggregate average volume per market movement  
- Compare volatility across trend types  
- Analyze distribution of increasing vs decreasing volume  
- Track monthly close price per trend category  
- Calculate trend-based high and low averages  

This step transformed row-level stock data into structured analytical summaries.

---

# 📈 Dashboard Architecture  

The dashboard consists of the following components:

---

## 🔢 Key Performance Indicators (KPIs)

- Total Trading Days Observed → **7,086**
- Volume Distribution Percentage
- Average Volume per Market Movement
- Maximum High & Minimum Low per Trend

---

## 📊 Visual Components  

### 1️⃣ Volume Distribution (Pie Chart)
Displays percentage of Increasing vs Decreasing trading volume.

**Insight:**  
Decreasing volume accounts for approximately **61%** of trading days.

---

### 2️⃣ Average Volume by Market Movement (Bar Chart)

Compares trading activity across:

- Bullish Days  
- Bearish Days  
- Neutral Days  

**Insight:**  
Bullish days show slightly higher average trading volume, indicating stronger investor participation during upward price movement.

---

### 3️⃣ Trend High/Low Comparison (Horizontal Bar Chart)

Analyzes volatility strength across:

- Confirmed Uptrend  
- Confirmed Downtrend  
- Unconfirmed Trends  

---

### 4️⃣ Monthly Close Price by Trend (Line Chart)

Tracks price evolution across trend categories over time.

---

### 5️⃣ Interactive Date Slicer  

Allows dynamic filtering by:

- Year  
- Period  
- Custom time ranges  

This transforms the dashboard into an exploratory analytical tool.

---

# 📷 Dashboard Preview  

## 🖥️ Main Dashboard  

![Amazon Dashboard](Amazon%20Stocks%20Dashboard.png)

---

## 📑 Raw Dataset Structure  

![Dataset Screenshot](Screenshot%202026-01-21%20164535.png)

---

# 📊 Key Analytical Insights  

### 🔎 Volume Behavior
- 61% of trading days show decreasing volume.
- Bullish days exhibit higher average volume than bearish days.
- Increasing volume combined with bullish movement may indicate momentum continuation.

---

### 🔎 Trend Reliability
- Confirmed trends demonstrate more consistent volatility structure.
- Unconfirmed trends show higher unpredictability.

---

### 🔎 Volatility Patterns
- Price Range metric highlights periods of high market uncertainty.
- High volatility aligns with directional market strength.

---

# 📈 Strategic Interpretation  

This analysis suggests:

- Volume acts as a supporting indicator of trend strength.
- Sustained bullish movement with rising volume signals institutional participation.
- Declining volume may precede consolidation or reversal.
- Confirmed trends provide stronger forecasting reliability than isolated movements.

---

# 🧠 Skills Demonstrated  

✔ Financial Data Analysis  
✔ Time Series Analysis  
✔ Feature Engineering  
✔ Trend Classification Modeling  
✔ Pivot Table Modeling  
✔ Interactive Dashboard Design  
✔ Data Storytelling  
✔ Business Insight Extraction  

---

# 💡 Tools & Technologies  

- Microsoft Excel  
  - Pivot Tables  
  - Calculated Columns  
  - IF Logic  
  - Interactive Slicers  
  - Data Visualization  

---

# 📂 Project Structure  

```
Amazon-Stock-Analysis/
│
├── Amazon_stock_data.xlsx
├── Amazon Stocks Dashboard.png
├── Screenshot 2026-01-21 164535.png
└── README.md
```

---

# 🚀 How to Use  

1. Download the repository  
2. Open `Amazon_stock_data.xlsx`  
3. Navigate to:
   - `Amazon_stock_data` → Cleaned dataset  
   - `Pivot Table` → Aggregated models  
   - `Dashboard` → Interactive visualization  

---

# 🔮 Future Improvements  

Potential enhancements:

- Add Moving Averages (MA20, MA50, MA200)
- Calculate Volatility Index
- Add CAGR analysis
- Incorporate RSI indicator
- Build Power BI version
- Convert to Python-based financial analysis project

---

# 👤 Author  

**Denzel Ayogu**  
Aspiring Data Analyst | Excel | SQL | Power BI  

---

⭐ If you found this project insightful, feel free to star the repository!
