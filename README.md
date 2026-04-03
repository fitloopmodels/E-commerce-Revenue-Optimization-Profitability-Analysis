# 🛒 E-commerce Revenue Optimization & Profitability Analysis

![Python](https://img.shields.io/badge/Python-3.10-blue?style=flat-square&logo=python)
![SQL](https://img.shields.io/badge/SQL-Advanced-orange?style=flat-square&logo=postgresql)
![Power BI](https://img.shields.io/badge/Power%20BI-Dashboard-yellow?style=flat-square&logo=powerbi)
![Machine Learning](https://img.shields.io/badge/ML-XGBoost-green?style=flat-square&logo=scikit-learn)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen?style=flat-square)

> Uncovering revenue patterns and profitability insights from 500,000+ transactional records using SQL, Python, and Power BI — with an XGBoost forecasting pipeline that cut RMSE by **21%**.

---

## 📌 Project Overview

This end-to-end data analytics project analyses the **Brazilian Olist E-commerce dataset** to identify revenue opportunities, optimize product strategy, and forecast future sales. The goal was to simulate the full workflow of a Data Analyst — from raw SQL queries to an executive-ready Power BI dashboard.

---

## 🎯 Business Objectives

- Identify top-performing products and underperforming SKUs
- Understand customer behavior through RFM segmentation
- Forecast monthly revenue with machine learning
- Deliver actionable recommendations for profitability improvement

---

## 🗂️ Dataset

| Detail | Info |
|---|---|
| Source | [Brazilian Olist Dataset – Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce) |
| Records | 500,000+ transactional rows |
| Tables | Orders, Products, Customers, Payments, Reviews |
| Period | 2016 – 2018 |

---

## 🔧 Tech Stack

| Layer | Tools |
|---|---|
| Data Querying | PostgreSQL / Advanced SQL |
| Data Processing | Python (Pandas, NumPy) |
| Machine Learning | XGBoost, Scikit-learn |
| Visualization | Matplotlib, Seaborn |
| BI Dashboard | Power BI (DAX, Power Query) |

---

## 📊 Key Analyses

### 1. 🧮 SQL — KPI Extraction
- Revenue trends by month, category, and region
- Customer Lifetime Value (CLV) calculation
- Category-level profit margin analysis using multi-stage aggregations and window functions

### 2. 👥 RFM Customer Segmentation (Python)
Built a **Recency, Frequency, Monetary (RFM)** model to segment customers into 4 groups:

| Segment | Description | Strategy |
|---|---|---|
| Champions | High R, F, M | Reward & retain |
| Loyal Customers | High F & M | Upsell opportunities |
| At-Risk | Low Recency | Re-engagement campaigns |
| Lost | Low R, F, M | Win-back or deprioritize |

### 3. 📈 XGBoost Revenue Forecasting
- Feature engineering: lag features, rolling averages, seasonality flags
- Benchmarked against baseline linear regression
- **Result: 21% reduction in RMSE** over baseline model

### 4. 📉 SKU Profitability Analysis
- Top 15% of products drove **68% of total revenue**
- Bottom 30% of SKUs operated at **negative margins**
- Delivered SKU rationalisation recommendations to eliminate low-margin drag

---

## 📐 Power BI Dashboard (6 Pages)

| Page | Content |
|---|---|
| 1. Executive Summary | Overall revenue, orders, and margin KPIs |
| 2. Sales Performance | Monthly trends and category breakdown |
| 3. Regional Heatmap | Revenue by state across Brazil |
| 4. Product Profitability | SKU-level margin analysis |
| 5. Customer Segments | RFM segment distribution |
| 6. Cohort Retention | Month-on-month customer retention rates |

---

## 💡 Key Findings

- 📦 Top 15% of products → 68% of revenue
- 🔴 Bottom 30% of SKUs → negative profit margins
- 📅 Revenue peaks in Q4 with a sharp November spike (Black Friday effect)
- 👤 "Champions" segment (8% of customers) contributed 41% of total GMV

---

## 📁 Repository Structure

```
📦 ecommerce-revenue-optimization
 ┣ 📂 sql
 ┃ ┣ kpi_queries.sql
 ┃ ┣ clv_analysis.sql
 ┃ └── margin_analysis.sql
 ┣ 📂 notebooks
 ┃ ┣ 01_eda.ipynb
 ┃ ┣ 02_rfm_segmentation.ipynb
 ┃ └── 03_xgboost_forecasting.ipynb
 ┣ 📂 powerbi
 ┃ └── dashboard.pbix
 ┣ 📂 data
 ┃ └── (download from Kaggle — link above)
 ┣ requirements.txt
 └── README.md
```

---

## 🚀 How to Run

```bash
# 1. Clone the repository
git clone https://github.com/fitloopmodels/ecommerce-revenue-optimization.git
cd ecommerce-revenue-optimization

# 2. Install dependencies
pip install -r requirements.txt

# 3. Download dataset from Kaggle and place CSVs in /data

# 4. Run notebooks in order (01 → 02 → 03)
jupyter notebook
```

---

## 📬 Contact

**Siva Prasath V M**
📧 sivaprasath.vm2003@gmail.com
🔗 [LinkedIn](https://www.linkedin.com/in/sivaprasathvm)
💻 [GitHub](https://github.com/fitloopmodels)
