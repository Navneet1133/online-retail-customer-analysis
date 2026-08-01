# Online Retail Sales & Customer Insights Analysis

Exploratory data analysis and RFM (Recency, Frequency, Monetary) customer segmentation on real
UK e-commerce transaction data, using Python, Pandas, and Matplotlib/Seaborn.

## Project Overview

This project analyzes ~500,000+ transaction records from a UK-based online retailer to answer
real business questions:

- How does revenue trend over time, and when are peak sales periods?
- Which countries and products drive the most revenue?
- Which customers are the most valuable, and which are at risk of churning?

## Dataset

**Online Retail II** — UCI Machine Learning Repository / Kaggle. Contains all transactions
between 01/12/2009 and 09/12/2011 for a UK-based, registered, non-store online retail company.

Download: search "Online Retail II UCI" on Kaggle, or fetch directly from the
[UCI Machine Learning Repository](https://archive.ics.uci.edu/dataset/502/online+retail+ii).

## Methodology

1. **Data Cleaning** — removed cancelled orders, invalid quantities/prices, missing customer IDs,
   and duplicate rows.
2. **Exploratory Analysis** — monthly revenue trends, country-level revenue breakdown, top
   products by revenue.
3. **RFM Segmentation** — scored each customer on Recency, Frequency, and Monetary value using
   quintile-based scoring, then classified customers into segments (Champions, Loyal Customers,
   Potential Loyalists, At Risk, Lost).

## Key Findings

See the notebook's final section for the full write-up with actual figures from this run. In
summary, a small segment of high-value ("Champion") customers accounts for a disproportionate
share of total revenue — a common pattern in retail businesses, with direct implications for
where to focus retention marketing spend.

## Tech Stack

- Python 3
- Pandas, NumPy
- Matplotlib, Seaborn
- Jupyter Notebook

## How to Run

```bash
pip install -r requirements.txt
jupyter notebook Online_Retail_EDA_RFM_Analysis.ipynb
```

Place the downloaded dataset file (`online_retail_II.csv` or `.xlsx`) in the same folder as the
notebook before running.

## Files

- `Online_Retail_EDA_RFM_Analysis.ipynb` — main analysis notebook
- `requirements.txt` — Python dependencies
- `customer_rfm_segments.csv` — RFM segment output per customer (one row per customer)

Note: the full cleaned transaction-level dataset (`cleaned_online_retail.csv`, ~780K rows) is not
included in this repo due to file size — it's regenerated automatically by running the notebook
end-to-end against the raw dataset.

## Author

Navneet Gujar
[LinkedIn](https://www.linkedin.com/in/navneet-gujar) | [GitHub](https://github.com/Navneet1133)
