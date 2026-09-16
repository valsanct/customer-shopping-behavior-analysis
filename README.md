# 🛍️ Customer Shopping Behavior Analysis

### Data Analyst Portfolio Project

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-336791?style=for-the-badge&logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![SQL](https://img.shields.io/badge/SQL-4479A1?style=for-the-badge&logo=mysql&logoColor=white)](https://www.w3schools.com/sql/)
[![Power BI](https://img.shields.io/badge/Power%20BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)](https://powerbi.microsoft.com/)
[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/)

---

## 📊 Project Overview

This project analyzes customer shopping behavior to understand purchasing patterns, customer segments, revenue, discounts, subscriptions, product performance, and purchasing preferences.

The dataset contains **3,900 records and 18 columns** covering:

- Customer demographics
- Purchase information
- Product categories
- Discounts
- Reviews
- Shipping
- Subscription status
- Previous purchases

The objective is to transform customer shopping data into actionable business insights using **Python, PostgreSQL, SQL, and Power BI**.

---

## 🎯 Business Problem

A retail company wants to understand customer shopping behavior to improve:

- Customer engagement
- Customer retention
- Marketing strategies
- Product strategies

### Business Question

> **How can customer shopping data be used to identify trends, improve customer engagement, and optimize marketing and product strategies?**

---

## 🔄 Project Workflow

The project follows an end-to-end data analytics workflow:

![Project Workflow](https://raw.githubusercontent.com/valsanct/customer-shopping-behavior-analysis/main/customer_shopping_behavior_analysis/5.images/workflow.png)   

**Raw Data → Python Data Preparation → PostgreSQL / SQL Business Analysis → Power BI Dashboard → Insights & Recommendations**

---

## 🛠️ Technologies Used

| Technology | Purpose |
|---|---|
| 🐍 **Python** | Data cleaning and transformation |
| 🐼 **Pandas** | Data manipulation and preparation |
| 🐘 **PostgreSQL** | Data storage and analysis |
| 🧮 **SQL** | Business analysis and customer segmentation |
| 📊 **Power BI** | Interactive dashboard and visualization |
| 🐙 **GitHub** | Version control and project documentation |

---

# 🧹 Data Preparation

The raw dataset was prepared using Python and Pandas.

### Key steps

- Inspected dataset structure and data quality
- Identified **37 missing Review Rating values**
- Imputed missing ratings using category-level median ratings
- Standardized column names using `snake_case`
- Created `age_group`
- Created `purchase_frequency_days`
- Removed redundant `promo_code_used`
- Loaded the cleaned data into PostgreSQL

---

# 🗄️ SQL Business Analysis

SQL was used to answer business questions related to:

### Revenue

- Revenue by gender
- Revenue by category
- Revenue by age group

### Customers

- Subscription vs. non-subscription behavior
- Customer loyalty
- Repeat purchases
- Customer segmentation

### Products

- Top products by rating
- Product rankings by category

### Purchasing Behavior

- Discount behavior
- Shipping preferences
- Discount-dependent products

---

## 👥 Customer Segmentation

Customers were segmented based on **Previous Purchases**:

| Customer Segment | Previous Purchases |
|---|---:|
| 🆕 **New** | 1 |
| 🔄 **Returning** | 2–10 |
| ⭐ **Loyal** | >10 |

This segmentation was used to analyze customer loyalty and revenue contribution across customer groups.

---

# 📊 Power BI Dashboard

The Power BI dashboard contains two pages focused on customer behavior, revenue, loyalty, and purchase drivers.

---

## 📌 Page 1 — Customer & Revenue Overview

Provides an overview of:

- Customer volume
- Revenue
- Subscription status
- Demographics
- Purchasing behavior

![Customer & Revenue Overview](https://raw.githubusercontent.com/valsanct/customer-shopping-behavior-analysis/main/customer_shopping_behavior_analysis/5.images/01.png)   

---

## 📌 Page 2 — Customer Behavior & Purchase Drivers

Examines:

- Discount behavior
- Shipping preferences
- Product ratings
- Customer segment revenue

![Customer Behavior & Purchase Drivers](https://raw.githubusercontent.com/valsanct/customer-shopping-behavior-analysis/main/customer_shopping_behavior_analysis/5.images/02.png)   

---

# 💡 Key Findings

- **3.9K** customer purchase records were analyzed.
- Approximately **27%** of customers are subscribers and **73%** are non-subscribers.
- Total revenue is approximately **$233K**.
- Overall average purchase is approximately **$59.76**.
- The **Loyal** customer segment contributes substantially more revenue than New and Returning customers in the current analysis.
- Gloves, sandals, boots, hat, and skirt have the highest average product ratings in the analysis.

---

# 📌 Business Recommendations

### 1. Increase Subscription Engagement

Evaluate targeted benefits and offers for non-subscribers.

### 2. Strengthen Customer Retention

Use targeted strategies to encourage progression from New to Returning and Loyal customers.

### 3. Review Discount Strategy

Evaluate discount usage by product and customer behavior to balance promotions with revenue objectives.

### 4. Promote Highly Rated Products

Use highly rated products in marketing and product-placement strategies.

### 5. Target Customer Segments

Use customer behavior and demographics to create more relevant marketing campaigns.

---

# 🎯 Business Answer

> **By analyzing who customers are, what they buy, how often they purchase, and which factors influence their spending, the company can identify trends, segment customers, personalize engagement, target marketing and promotions, and optimize its product strategy.**

---

# 📁 Repository Structure

```text
customer-shopping-behavior-analysis/
│
├── data/
│   └── customer_shopping_behavior.csv
│
├── python/
│   └── data_preparation.py
│
├── sql/
│   └── business_analysis.sql
│
├── powerbi/
│   └── customer_shopping_behavior.pbix
│
├── report/
│   └── customer_shopping_behavior_report.pdf
│
├── images/
│   ├── dashboard_page_1.png
│   ├── dashboard_page_2.png
│   └── workflow.png
│
└── README.md
