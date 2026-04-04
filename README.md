# 📊 Customer Shopping Behavior Analysis
![Python](https://img.shields.io/badge/Python-3776AB?style=flat&logo=python&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=flat&logo=postgresql&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-150458?style=flat&logo=pandas&logoColor=white)
![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=flat&logo=powerbi&logoColor=black)
![SQL](https://img.shields.io/badge/SQL-CC2927?style=flat&logo=microsoftsqlserver&logoColor=white)

> **End-to-End Data Analytics Project — Retail Customer Behavior**

A complete data analytics project analyzing **3,900 retail transactions** to uncover insights into customer spending patterns, product preferences, discount behavior and subscription trends. Built using Python, PostgreSQL and Power BI.

---

## 📈 Key Numbers

| Metric | Value |
|--------|-------|
| Total Transactions | 3,900 |
| Dataset Features | 18 columns |
| SQL Queries Written | 10 |
| Male Revenue | $157,890 |
| Female Revenue | $75,191 |
| Loyal Customers | 3,116 |
| Returning Customers | 701 |
| New Customers | 83 |
| High-Value Discount Users | 839 |
| Top Revenue Segment | Young Adults ($62,143) |
| Avg Purchase Amount | $59.76 |
| Avg Review Rating | 3.75 |

---

## 🚀 Quick Start

```bash
# 1. Clone the repository
git clone https://github.com/Smit-Velani/customer_behavior.git

# 2. Install dependencies
pip install pandas psycopg2 sqlalchemy

# 3. Run the Python notebook
jupyter notebook Customer_Shopping_Behavior_Analysis.ipynb

# 4. Execute SQL queries
# Run customer_behavior_sql_queries.sql in pgAdmin or PostgreSQL
```

---

## 📁 Project Structure

```
Customer_Shopping_Behavior_Analysis/
│
├── Customer_Shopping_Behavior_Analysis.ipynb  ← Python EDA & cleaning
├── customer_behavior_sql_queries.sql          ← 10 business SQL queries
├── customer_shopping_behavior.csv             ← Raw dataset
├── Business Problem Document.pdf             ← Problem statement
├── Customer Shopping Behavior Analysis.pdf   ← Full project report
├── LICENSE
└── README.md
```

---

## ⚙️ Project Workflow

### 1️⃣ Data Preparation (Python + Pandas)

- Imported dataset and explored with `df.info()` and `.describe()`
- Handled **37 missing values** in Review Rating using median imputation per category
- Standardized column names to **snake_case**
- Engineered **age_group** column by binning customer ages
- Created **purchase_frequency_days** feature
- Dropped redundant `promo_code_used` column
- Connected Python to **PostgreSQL** and loaded cleaned DataFrame

### 2️⃣ Data Analysis (SQL — 10 Business Queries)

| # | Query | Result |
|---|-------|--------|
| Q1 | Revenue by Gender | Male: $157,890 · Female: $75,191 |
| Q2 | High-Spending Discount Users | **839 customers** above average spend |
| Q3 | Top 5 Products by Rating | Gloves (3.86) · Sandals (3.84) · Boots (3.82) |
| Q4 | Shipping Type Comparison | Express: $60.48 · Standard: $58.46 avg spend |
| Q5 | Subscribers vs Non-Subscribers | 1,053 subscribers · 2,847 non-subscribers |
| Q6 | Products with Highest Discount Usage | Hat (50%) · Sneakers (49.66%) · Coat (49.07%) |
| Q7 | Customer Segmentation | **3,116 Loyal** · 701 Returning · 83 New |
| Q8 | Top 3 Products per Category | Jewelry · Blouse · Sandals top in each category |
| Q9 | Repeat Buyers & Subscriptions | 958 repeat buyers subscribed |
| Q10 | Revenue by Age Group | Young Adults: **$62,143** (highest) |

### 3️⃣ Dashboard Visualization (Power BI)

Interactive dashboard built with:
- Revenue distribution by category and gender
- Customer segmentation breakdown
- Age group revenue contribution
- Subscription status analysis
- Purchase behavior trends

---

## 📊 Key Insights

- **Young Adults** are the top revenue segment contributing **$62,143**
- **Male customers** generate 2× more revenue than female ($157K vs $75K)
- **839 customers** used discounts but still spent above average — high-value segment
- **Loyal customers (3,116)** dominate — loyalty programs would boost retention
- **Express shipping users** spend more on average ($60.48 vs $58.46)
- Top products by rating: **Gloves (3.86), Sandals (3.84), Boots (3.82)**

---

## 💡 Business Recommendations

| Recommendation | Action |
|----------------|--------|
| **Boost Subscriptions** | Promote exclusive benefits to non-subscribers (2,847) |
| **Customer Loyalty Programs** | Reward repeat buyers to retain 3,116 loyal customers |
| **Review Discount Strategy** | Balance discounts — 839 high-spenders still buy at discount |
| **Product Positioning** | Promote top-rated products (Gloves, Sandals, Boots) |
| **Targeted Marketing** | Focus on Young Adults and Express shipping users |

---

## 🔑 SQL Techniques Used

| Technique | Usage |
|-----------|-------|
| `GROUP BY` + `SUM` | Revenue aggregation by gender and age group |
| `CTE` | Customer segmentation logic |
| `Window Functions` | Top 3 products per category using `ROW_NUMBER()` |
| `Subquery` | High-spending discount users above average |
| `CASE WHEN` | New / Returning / Loyal classification |
| `HAVING` | Filtering discount-heavy products |

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|------|---------|
| `Python` | Data preparation and feature engineering |
| `Pandas` | DataFrame manipulation and cleaning |
| `PostgreSQL` | Business SQL analysis |
| `Power BI` | Interactive dashboard visualization |
| `Jupyter Notebook` | EDA and documentation |

---

## 👤 Author

**Smit Velani**
Data Science MS — Northeastern University

---

*Built with Python · Pandas · PostgreSQL · Power BI*

