# Trader Performance vs Market Sentiment Analysis

## Primetrade.ai – Data Science / Analytics Intern Assignment

### Overview

This project analyzes the relationship between Bitcoin market sentiment (Fear & Greed Index) and trader behavior on Hyperliquid. The objective is to investigate whether market sentiment influences trader profitability, trading activity, and overall trading behavior, and to derive actionable trading strategies based on the analysis.

---

## Project Objectives

- Clean and preprocess the provided datasets.
- Merge market sentiment data with historical trading data.
- Analyze trader performance under different market sentiment conditions.
- Identify behavioral patterns among different trader segments.
- Generate insights supported by visualizations and statistical summaries.
- Recommend practical trading strategies based on the findings.

---

## Datasets

### 1. Bitcoin Fear & Greed Index
Contains daily Bitcoin market sentiment.

**Columns include:**
- Date
- Classification (Fear, Greed, Extreme Fear, Extreme Greed)
- Sentiment Score

### 2. Hyperliquid Historical Trader Data
Contains historical trading activity.

**Key fields include:**
- Account
- Coin
- Side
- Execution Price
- Size (USD)
- Closed PnL
- Timestamp

---

## Technologies Used

- Python 3.x
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Project Structure

```
Trader-Performance-vs-Market-Sentiment/
│
├── data/
│   ├── fear_greed.csv
│   └── historical_data.csv
│
├── outputs/
│   ├── charts/
│   └── tables/
│
├── Trader_Performance_Analysis.ipynb
├── README.md
└── requirements.txt
```

---

## Methodology

### 1. Data Preparation
- Loaded both datasets.
- Checked data types, missing values, and duplicates.
- Converted timestamps into datetime format.
- Created a common date column.
- Merged trader data with daily market sentiment.

### 2. Feature Engineering
Generated analytical features including:
- Daily Profit & Loss (PnL)
- Trade Count
- Average Trade Size
- Win Rate
- Trader Segmentation
- Drawdown Proxy

### 3. Exploratory Data Analysis
Performed analysis using:
- Average PnL by sentiment
- Trade size distribution
- Trading frequency
- BUY vs SELL ratio
- Correlation heatmap

### 4. Trader Segmentation
Segmented traders into:
- Frequent vs Infrequent Traders
- Top Performers vs Other Traders

---

## Key Findings

- Extreme Greed periods showed the highest average trader profitability.
- Extreme Fear periods showed comparatively weaker trading performance.
- Trading activity increased significantly during Fear periods.
- Frequent traders did not necessarily achieve higher profitability than infrequent traders.
- Market sentiment alone was not a strong predictor of individual trade profitability.

---

## Strategy Recommendations

- Reduce position size and strengthen risk management during Extreme Fear periods.
- Consider maintaining exposure during Extreme Greed while following disciplined profit-taking strategies.
- Prioritize trade quality over trade frequency, as excessive trading did not consistently improve profitability.

---

## Output Files

### Charts
- Average PnL by Market Sentiment
- Trade Size Distribution
- Trade Frequency by Sentiment
- Correlation Heatmap
- Closed PnL Distribution

### Tables
- Sentiment Summary
- Trader Segments
- Performance Summary
- Drawdown Proxy
- Daily PnL
- Trade Count
- Average Trade Size
- Win Rate

---

## Limitations

The provided Hyperliquid dataset does not include leverage information. Therefore, leverage distribution analysis could not be performed.

---

## How to Run

### 1. Clone the repository

```bash
git clone <repository-url>
cd Trader-Performance-vs-Market-Sentiment
```

### 2. Install dependencies

```bash
pip install -r requirements.txt
```

### 3. Place the datasets

Copy the following files into the **data/** directory:

- fear_greed.csv
- historical_data.csv

### 4. Run the notebook

Open:

```
Trader_Performance_Analysis.ipynb
```

Run all cells sequentially.

---

## Future Improvements

- Include leverage-based analysis if leverage data becomes available.
- Develop predictive models for trader profitability.
- Build an interactive dashboard using Streamlit or Power BI.
- Apply clustering techniques to identify additional trader archetypes.

---

## Author

Prepared as part of the **Primetrade.ai Data Science / Analytics Intern – Round 0 Assignment**.