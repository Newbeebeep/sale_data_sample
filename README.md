# 🛍️ Sales Data Analysis Capstone Project

This project is a capstone data analysis exercise inspired by a classmate's final project structure. The goal is to use business retail sales data to explore performance trends, identify top/bottom-performing products, and provide actionable recommendations for product line optimization and business growth.

---

## 📌 Project Objectives

- Analyze overall sales performance across time, product lines, and regions.
- Identify the top-selling products and underperforming items.
- Explore seasonal trends and country-wise performance.
- Investigate product return rates and their business impact.
- Provide strategic suggestions to discontinue low-performing products and expand high-performing ones.

---

## 🗂️ Dataset Description

**Source**: [Kaggle - Sales Data (Walmart-style)](https://www.kaggle.com/datasets/kyanyoga/sample-sales-data)  
**File**: `sales_data_sample.csv`  
**Total Rows**: ~2800  
**Fields**:

| Column Name | Description |
|-------------|-------------|
| ORDERNUMBER | Unique order ID |
| QUANTITYORDERED | Number of items ordered |
| PRICEEACH | Unit price of product |
| SALES | Total value of the order line |
| ORDERDATE | Order date |
| STATUS | Order status (Shipped, Cancelled, etc.) |
| PRODUCTLINE | Product category |
| CUSTOMERNAME | Customer name |
| COUNTRY | Country of customer |
| DEALSIZE | Deal size classification (Small/Medium/Large) |
| ... | (See full dataset for more fields) |

---

## 🔍 Key Business Questions

1. Which product lines generate the highest revenue?
2. Which specific products generate the lowest sales and may need to be discontinued?
3. Which products are most frequently returned?
4. How does monthly or quarterly revenue trend over time?
5. Which customers or countries contribute most to revenue?
6. What is the revenue distribution by deal size?

---

## ✅ Data Cleaning Summary

- Converted `ORDERDATE` to datetime format.
- Extracted `YEAR`, `MONTH`, `QUARTER` for time-based analysis.
- Handled missing values:
  - Filled missing `STATE` and `TERRITORY` with "Unknown".
  - Dropped unnecessary column `ADDRESSLINE2` with 89% nulls.
  - Filled missing postal codes with `0`.

---

## 📊 Exploratory Data Analysis (EDA)

- Grouped sales by `PRODUCTLINE` to identify top-performing categories.
- Analyzed product cancellations by status = 'Cancelled'.
- Built a recommendation system to identify low-performing products for potential discontinuation based on sales and quantity.

---

## ✅ Key Insights

- Top-selling product lines are **Classic Cars**, followed by **Vintage Cars** and **Motorcycles**.
- No products met the criteria for discontinuation based on both low revenue and low quantity.
- This suggests a **healthy product portfolio**, but certain products with high cancellation counts are flagged for future monitoring.
- Most returned product lines include **Ships**, **Planes**, and **Classic Cars**.
- Quarter 3 shows the highest overall revenue across all recorded years.

---

## 📈 Tableau Dashboard (In Progress)

A visual dashboard was built in Tableau to summarize the analysis.

🔗 [View Tableau Dashboard](#) _(Link will be updated when published)_

Suggested charts:
- Sales by Product Line
- Monthly Sales Trend
- Country-wise Sales Distribution
- Top Returned Products
- Product Discontinuation Watchlist

---

## 📄 Project Structure

```
MyCapstone_SalesAnalysis/
│
├── data/                         ← Raw + cleaned data
├── notebooks/                    ← Jupyter analysis notebooks
├── dashboard/                    ← Tableau dashboard
├── presentations/                ← Final presentation slides
├── README.md                     ← You're reading it!
└── .gitignore
```

---

## 👩‍💼 Author

**Your Name**  
Nashville Software School – Data Analytics Cohort  
GitHub: [your-github-link]  
LinkedIn: [your-linkedin-link]

