# Bitcoin Market Sentiment vs Trader Performance Analysis

## Project Overview

This project analyzes the relationship between Bitcoin market sentiment and trader performance using the Bitcoin Fear & Greed Index and  historical trading data.

The objective is to identify how market sentiment influences trading activity, profitability, and trading behavior.

---

## Datasets Used

### 1. Bitcoin Market Sentiment Dataset
Columns:
- Date
- Classification (Extreme Fear, Fear, Neutral, Greed, Extreme Greed)

### 2.Historical Trader Dataset
Columns:
- Account
- Symbol
- Side (BUY/SELL)
- Closed PnL
- Timestamp
- Trade Information



### Data Cleaning
- Checked missing values
- Removed duplicate records
- Converted timestamp columns to datetime format
- Created a date column for analysis
- Merged both datasets using the date field

### Exploratory Data Analysis (EDA)
- Sentiment distribution analysis
- Average profit by sentiment
- Total profit by sentiment
- BUY vs SELL performance analysis
- Trading activity analysis


### Trading Activity by Sentiment

| Sentiment | Number of Trades |
|------------|----------------|
| Fear | 13,869 |
| Greed | 11,292 |
| Extreme Greed | 5,621 |
| Neutral | 2,756 |
| Extreme Fear | 2,326 |

**Insight:** Fear periods recorded the highest trading activity.

---

### Average Profit by Sentiment

| Sentiment | Average Closed PnL |
|------------|------------------|
| Extreme Greed | 205.82 |
| Fear | 128.29 |
| Greed | 53.99 |
| Neutral | 27.09 |
| Extreme Fear | 1.89 |

**Insight:** Extreme Greed generated the highest average profit per trade.

---

### Total Profit by Sentiment

| Sentiment | Total Closed PnL |
|------------|----------------|
| Fear | 1,779,226 |
| Extreme Greed | 1,156,894 |
| Greed | 609,633 |
| Neutral | 74,657 |
| Extreme Fear | 4,400 |

**Insight:** Fear periods generated the highest overall profit because of significantly higher trading activity.

---

### BUY vs SELL Performance

| Side | Average Closed PnL |
|------|------------------|
| BUY | 36.10 |
| SELL | 60.71 |

**Insight:** SELL trades outperformed BUY trades by approximately 68%.

---

## Hidden Patterns Discovered

- Fear periods generated the highest trading activity.
- Extreme Greed produced the highest average profitability.
- SELL positions consistently outperformed BUY positions.
- Extreme Fear conditions resulted in very low profitability.
- Market sentiment significantly influenced trader performance.

---

## Recommendations

1. Use sentiment indicators as part of trading strategies.
2. Exercise caution during Extreme Fear periods.
3. Consider momentum-based strategies during Extreme Greed periods.
4. Monitor Fear periods closely as they generated the highest overall profits.
5. Evaluate short-selling opportunities as SELL trades showed stronger performance.

---

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Project Structure

```
assignment/
│
├── analysis.ipynb
├── historical_data.csv
├── fear_greed_index.csv
├── README.md
└── requirements.txt
```

---

## Conclusion

This analysis demonstrates a strong relationship between Bitcoin market sentiment and trader performance. Fear periods generated the highest trading activity and total profits, while Extreme Greed delivered the highest average profit per trade. The findings suggest that combining sentiment analysis with historical trading data can support better trading decisions and risk management.

---

## Author

**Sangram Pardhe**

Aspiring Data Analyst | Python | SQL | Power BI | Data Visualization