# Amazon Stock Prediction & Analysis

An end-to-end exploratory data analysis and feature engineering project on Amazon (AMZN) historical stock data spanning **24 years (1997–2021)**. This project demonstrates applied data science skills including financial data ingestion, time-series preprocessing, and visualization-driven insight generation.

---

## Outcomes & Key Findings

- Analyzed **6,076 trading days** of AMZN stock data across Open, High, Low, Close, Adjusted Close, and Volume
- Engineered a **Daily Return** feature to quantify day-over-day price volatility and momentum
- Identified long-term growth trends and volatility patterns across different market periods (dot-com boom/bust, 2008 recession, COVID-era surge)
- Produced multi-variable subplot visualizations revealing structural changes in trading volume and price behavior over time

---

## Tech Stack

| Tool | Purpose |
|---|---|
| Python 3 | Core programming language |
| Jupyter Notebook | Interactive development environment |
| `yfinance` | Automated download of historical AMZN stock data from Yahoo Finance |
| `pandas` | Data wrangling, feature engineering, time-series manipulation |
| `matplotlib` | Multi-panel financial visualizations |

---

## How It Was Built

### 1. Data Ingestion
Historical AMZN ticker data was pulled programmatically using `yfinance`, covering May 1997 through July 2021 — the full public trading history at the time of analysis.

### 2. Preprocessing
- Renamed columns for readability
- Converted date strings to `datetime` objects and sorted chronologically
- Extracted month from the date for temporal analysis
- Removed null values introduced during feature creation

### 3. Feature Engineering
- **Daily Return**: Computed as the percentage change in closing price between consecutive trading days — a standard metric for measuring short-term momentum and volatility

### 4. Exploratory Analysis & Visualization
- Generated a 9-panel subplot grid covering all key variables across the full 24-year timeline
- Examined price movement, volume spikes, and return distributions to surface market behavior patterns

---

## Project Structure

```
amazonstockprediction/
├── Amazon_Stock_Prediction.ipynb   # Full analysis notebook
└── README.md
```

---

## Getting Started

```bash
# Install dependencies
pip install yfinance pandas matplotlib jupyter

# Launch notebook
jupyter notebook Amazon_Stock_Prediction.ipynb
```

---

## About

Built as part of a data science portfolio to demonstrate practical skills in financial data analysis, time-series feature engineering, and communicating insights through visualization.
