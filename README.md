# 🧠📊 CBIA — Customer Behavior Intelligence & Analytics

![SQL](https://img.shields.io/badge/SQL-MySQL-blue)
![Python](https://img.shields.io/badge/Python-Analysis-yellow)
![PowerBI](https://img.shields.io/badge/Dashboard-PowerBI-orange)
![Excel](https://img.shields.io/badge/Data_Prep-Excel-brightgreen)
![DAX](https://img.shields.io/badge/DAX-Measures-red)
![ML](https://img.shields.io/badge/ML-Scikit--Learn-purple)
![Level](https://img.shields.io/badge/Level-Intermediate--Advanced-green)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![GitHub last commit](https://img.shields.io/github/last-commit/mr-deepak-kp/CBIA)
![GitHub repo size](https://img.shields.io/github/repo-size/mr-deepak-kp/CBIA)
![GitHub stars](https://img.shields.io/github/stars/mr-deepak-kp/CBIA?style=social)
![GitHub forks](https://img.shields.io/github/forks/mr-deepak-kp/CBIA?style=social)

---

## 📌 Project Overview

**CBIA (Customer Behavior Intelligence & Analytics)** is a full-scale, enterprise-grade data analytics project that delivers deep insights into customer behavior, segmentation, lifetime value, and churn prediction for **XYZ Pvt. Ltd.**

The project analyzes **5,000 customers** across **22 behavioral features** spanning **2 years (Jan 2023 – Dec 2024)**, applying advanced Machine Learning models and delivering a **5-page interactive Power BI Dashboard** with full navigation, DAX measures, and dynamic slicers.

The solution combines **RFM Scoring**, **KMeans Clustering**, **CLV Prediction**, and **Churn Modeling** into a single cohesive analytics platform — enabling data-driven decisions around revenue growth, customer retention, and marketing optimization.

---

## 🎯 Objectives

- 👥 Segment 5,000 customers using RFM scoring + KMeans clustering into 5 behavioral groups
- 💎 Predict Customer Lifetime Value (CLV) using Gradient Boosting regression
- ⚠️ Identify churned and at-risk customers using ML classification models
- 📊 Build a 5-page interactive Power BI dashboard with navigation and DAX KPIs
- 🗄️ Create a SQL analytics layer with KPI views and window function queries
- 📈 Deliver actionable insights aligned with BRD business targets

---

## 🔗 Quick Links

| Resource | Link |
|----------|------|
| 📊 Power BI Dashboard (.pbix) | [View Dashboard](https://github.com/mr-deepak-kp/CBIA) |
| 🌐 CBIA Dashboard Preview (HTML) | [View Live Preview](https://github.com/mr-deepak-kp/CBIA) |
| 📄 BRD Document | [Download BRD](https://github.com/mr-deepak-kp/CBIA) |
| 🐍 Python Notebooks | [View Notebooks](https://github.com/mr-deepak-kp/CBIA) |

---

## 📁 Project Structure

```
CBIA — Customer Behavior Intelligence & Analytics/
│
├── 📄 data/
│   ├── customer_shopping_behavior.csv        # Raw dataset (original)
│   ├── customer_cleaned.csv                  # Cleaned & processed dataset
│   ├── rfm_scored.csv                        # RFM scores per customer
│   ├── customers_segmented.csv               # KMeans segment labels
│   ├── clv_predictions.csv                   # CLV predictions per customer
│   └── churn_predictions.csv                 # Churn labels & probabilities
│
├── 🐍 notebooks/
│   ├── 01_EDA_Data_Cleaning.ipynb            # Exploratory data analysis & cleaning
│   ├── 02_RFM_Scoring.ipynb                  # RFM scoring logic
│   ├── 03_KMeans_Clustering.ipynb            # KMeans segmentation
│   ├── 04_CLV_Prediction.ipynb               # CLV prediction model
│   └── 05_Churn_Model.ipynb                  # Churn prediction model
│
├── 🗄️ sql/
│   └── 06_SQL_Scripts_MySQL.sql              # Full SQL analytics layer & KPI views
│
├── 📊 dashboard/
│   └── CBIA_Dashboard.pbix                   # Power BI Dashboard (5 pages)
│
├── 🌐 CBIA_Dashboard_Code/                   # ← Dashboard HTML Preview
│   └── CBIA_dashboard_preview.html           # Interactive 5-page dashboard preview
│
├── 🖼️ Dashboard_Images/                      # ← Dashboard Screenshots
│   ├── dashboard_image1.png                  # Page 1 — Executive KPIs
│   ├── dashboard_image2.png                  # Page 2 — Customer Intelligence
│   ├── dashboard_image3.png                  # Page 3 — Sales Analytics
│   ├── dashboard_image4.png                  # Page 4 — Churn Analysis
│   └── dashboard_image5.png                  # Page 5 — CLV & Loyalty
│
├── 📁 outputs/
│   ├── customer_cleaned.xlsx                 # Master cleaned data export
│   ├── rfm_scores.xlsx                       # RFM scores export
│   ├── clv_predictions.xlsx                  # CLV predictions export
│   ├── winback_list.xlsx                     # Top at-risk win-back list
│   └── eda_overview.png                      # EDA chart exports
│
├── 📑 docs/
│   ├── Customer_Behavior_BRD_v2.docx         # Business Requirements Document
│   └── CBIA_Presentation.pptx               # Project presentation deck
│
└── 📝 README.md                              # Project documentation
```

---

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| ![MySQL](https://img.shields.io/badge/MySQL-Database-blue) | Data storage, schema design, KPI views, window functions |
| ![Python](https://img.shields.io/badge/Python-ML_&_EDA-yellow) | EDA, RFM scoring, KMeans, CLV & churn prediction |
| ![Power BI](https://img.shields.io/badge/PowerBI-Dashboard-orange) | 5-page interactive dashboard, DAX measures, navigation |
| ![Excel](https://img.shields.io/badge/Excel-Data_Export-brightgreen) | Master data export, deliverable formatting |
| ![DAX](https://img.shields.io/badge/DAX-Measures-red) | KPI calculations, segment filters, dynamic measures |
| ![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-ML-purple) | KMeans, Logistic Regression, Gradient Boosting |
| ![Pandas](https://img.shields.io/badge/Pandas-Analysis-lightblue) | Data manipulation, transformation, feature engineering |
| ![Matplotlib](https://img.shields.io/badge/Matplotlib-Visualization-blue) | EDA charts and visual outputs |
| ![Seaborn](https://img.shields.io/badge/Seaborn-Visualization-teal) | Statistical and correlation visualizations |

---

## 🗄️ Database Schema

```sql
CREATE DATABASE customer_behavior;
USE customer_behavior;

CREATE TABLE customer_data (
    Customer_ID             INT,
    Age                     INT,
    Age_Group               VARCHAR(20),
    Gender                  VARCHAR(15),
    Location                VARCHAR(50),
    Order_ID                VARCHAR(20),
    Order_Date              DATE,
    Item_Purchased          VARCHAR(100),
    Category                VARCHAR(60),
    Quantity                INT,
    Purchase_Amount_USD     DECIMAL(10,2),
    Discount_Applied        VARCHAR(10),
    Revenue                 DECIMAL(10,2),
    Payment_Method          VARCHAR(40),
    Shipping_Type           VARCHAR(30),
    Season                  VARCHAR(20),
    Review_Rating           DECIMAL(3,1),
    Subscription_Status     VARCHAR(10),
    Previous_Purchases      INT,
    Frequency_of_Purchases  VARCHAR(50),
    Size                    VARCHAR(10),
    Color                   VARCHAR(30)
);
```

---

## 🧠 ML Models Used

| Model | Purpose | Result |
|-------|---------|--------|
| **KMeans Clustering** | Customer segmentation into 5 groups | 5 clean segments |
| **Gradient Boosting** | CLV prediction (best performer) | R² = 0.61 |
| **Random Forest** | Churn prediction | AUC-ROC = 1.0 |
| **Logistic Regression** | Churn baseline model | Compared against RF |
| **RFM Scoring** | Rule-based segmentation | R, F, M scores (1–5) |

---

## 📊 Dashboard Pages — 5 Pages

| Page | Title | Key Charts |
|------|-------|-----------|
| **P1** | Executive KPIs | Revenue · Churn Rate · AOV · KPI Gauges · YoY |
| **P2** | Customer Intelligence | RFM Scatter · Segment Bar · Donut · Top 5 Table |
| **P3** | Sales Analytics | Monthly Trend · Category · Heatmap · Payment |
| **P4** | Churn Analysis | Gauge · Win-Back List · Subscription · Age Group |
| **P5** | CLV & Loyalty | Loyalty Funnel · CLV Segment · Tier Donut · Top 10 |

---

## 📋 SQL Scripts — Analytics Layer

### KPI Validation
```sql
SELECT * FROM vw_kpi_summary;
-- Returns: total_customers, total_revenue,
--          avg_clv, churn_rate_pct, repeat_customer_rate_pct
```

### Revenue Analytics
```sql
-- Revenue by Category
SELECT Category, SUM(Revenue) AS Total_Revenue
FROM customer_data
GROUP BY Category
ORDER BY Total_Revenue DESC;
```

### RFM SQL Layer
```sql
-- RFM Scoring with Window Functions
SELECT Customer_ID,
    DATEDIFF('2024-12-31', MAX(Order_Date)) AS Recency,
    COUNT(Order_ID)                          AS Frequency,
    SUM(Revenue)                             AS Monetary,
    NTILE(5) OVER (ORDER BY SUM(Revenue))    AS M_Score
FROM customer_data
GROUP BY Customer_ID;
```

### Churn Analytics
```sql
-- At-Risk Customers
SELECT Customer_ID, Recency, Frequency, Monetary
FROM customer_data
WHERE DATEDIFF('2024-12-31', MAX(Order_Date)) > 180
GROUP BY Customer_ID;
```

> 📄 Full scripts available in [`sql/06_SQL_Scripts_MySQL.sql`](sql/06_SQL_Scripts_MySQL.sql)

---

## 🧠 Skills Demonstrated

| Skill | Description |
|-------|-------------|
| **RFM Scoring** | Quintile-based R, F, M scoring (1–5 scale) |
| **KMeans Clustering** | Elbow method, Silhouette score, PCA visualization |
| **CLV Prediction** | 4 model comparison — Gradient Boosting best |
| **Churn Modeling** | Binary classification, AUC-ROC, feature importance |
| **SQL Analytics** | Window functions, CTEs, RANK(), KPI views |
| **DAX Measures** | DIVIDE, CALCULATE, FILTER, dynamic KPI cards |
| **Power BI** | 5-page dashboard, navigation, slicers, drill-through |
| **EDA** | Univariate, bivariate, correlation, outlier analysis |
| **Python** | pandas, sklearn, matplotlib, seaborn |
| **Documentation** | BRD, PPT, README, SQL query documentation |

---

## 📊 Key Findings

| Metric | Value |
|--------|-------|
| 👥 Total Customers | 5,000 |
| 💰 Total Revenue | $1.96M |
| 📈 YoY Revenue Growth | +32% (2023 → 2024) |
| ⚠️ Churn Rate | 42.7% (Target: 27%) |
| 🔄 Retention Rate | 99.7% |
| 💎 Total Predicted CLV | $5.18M |
| 📦 Avg Order Value | $393 |
| 🏆 Avg CLV / Customer | $1,035 |

### 💡 Segment Insights

| Segment | Customers | Churn Rate | Avg CLV |
|---------|-----------|-----------|---------|
| Champion | 246 (5%) | 13% | $2,084 |
| Loyal | 1,293 (26%) | 16% | $1,682 |
| Potential | 1,250 (25%) | 50% | $563 |
| At-Risk | 1,100 (22%) | 45% | $1,815 |
| Lost | 1,111 (22%) | 73% | $267 |

### ⚠️ Critical Findings

- **42.7% churn rate** — 15.7% above target of 27%
- **$624K revenue at risk** from churned customers
- **Subscribers churn 36.8% less** than non-subscribers
- **Fall season** drives highest revenue — $560K (29%)
- **Clothing category** leads at $777K — 40% revenue share
- **Champions (5%)** contribute **40%+** of total revenue

---

## 🐍 Python Analysis — 5 Notebooks

| Notebook | Key Tasks |
|----------|-----------|
| **01_EDA_Data_Cleaning** | Data loading, null handling, duplicates, EDA charts (12 visuals) |
| **02_RFM_Scoring** | Recency, Frequency, Monetary calculation, 1–5 scoring |
| **03_KMeans_Clustering** | Elbow method, Silhouette, PCA, 5 segment labels |
| **04_CLV_Prediction** | 4 model comparison, Gradient Boosting, CLV tiers |
| **05_Churn_Model** | Random Forest vs Logistic Regression, AUC-ROC, win-back list |

---

## 📑 Business Requirements — KPI Targets

| Objective | Target | KPI Measured |
|-----------|--------|-------------|
| Revenue Growth | +20% | Total Revenue |
| Churn Reduction | -15% | Churn Rate |
| Retention Improvement | +10% | Repeat Customer Rate |
| AOV Increase | +12% | Average Order Value |
| CLV Optimization | +18% | Predicted CLV |

---

## 📑 Project Deliverables

| # | Deliverable | Format | Status |
|---|-------------|--------|--------|
| 1 | Business Requirements Document | `.docx` | ✅ Complete |
| 2 | Customer Dataset (Cleaned) | `.csv / .xlsx` | ✅ Complete |
| 3 | Python EDA & ML Notebooks × 5 | `.ipynb` | ✅ Complete |
| 4 | SQL Analytics Scripts | `.sql` | ✅ Complete |
| 5 | Power BI Dashboard | `.pbix` | ✅ Complete |
| 6 | Dashboard HTML Preview | `.html` | ✅ Complete |
| 7 | Dashboard Screenshots × 5 | `.png` | ✅ Complete |
| 8 | Project Presentation | `.pptx` | ✅ Complete |
| 9 | GitHub Repository | Public | ✅ Complete |

---

## 🔮 Future Improvements

- [ ] Publish Power BI dashboard to Power BI Service for live access
- [ ] Build real-time churn alert system using streaming data
- [ ] Add A/B testing framework for marketing campaigns
- [ ] Integrate CRM system for automated win-back triggers
- [ ] Expand CLV model with BG/NBD probabilistic approach
- [ ] Add cohort retention analysis by acquisition month
- [ ] Build automated weekly KPI report using SQL stored procedures
- [ ] Deploy ML models as REST API using FastAPI

---

## 🤝 Connect With Me

[![GitHub](https://img.shields.io/badge/GitHub-mr--deepak--kp-181717?style=for-the-badge&logo=github)](https://github.com/mr-deepak-kp)    
[![LinkedIn](https://img.shields.io/badge/LinkedIn-deepak--kumar--prasad-0A66C2?style=for-the-badge&logo=linkedin)](https://www.linkedin.com/in/deepak-kumar-prasad/)

---

>   🧠 CBIA · MySQL · Python · Power BI · Excel · DAX · Machine Learning · XYZ Pvt. Ltd. · May 2026 · Deepak Kumar Prasad
       
