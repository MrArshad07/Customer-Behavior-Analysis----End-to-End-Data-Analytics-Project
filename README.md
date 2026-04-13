# 🛍️ Customer Behavior Analysis – End-to-End Data Analytics Project

## 📌 Project Overview

This project is a complete **end-to-end data analysis pipeline** that focuses on understanding customer shopping behavior and generating actionable business insights.

The analysis covers:

* Customer segmentation
* Revenue drivers
* Discount effectiveness
* Subscription impact
* Product performance

This project demonstrates real-world data analytics skills aligned with **industry standards (Amazon-level analytics thinking)**.

---

## 🧰 Tech Stack

* 🐍 Python (Pandas, NumPy, Matplotlib, Seaborn)
* 🗄️ SQL (MySQL)
* 📊 Power BI (Dashboard + DAX)
* 📓 Jupyter Notebook

---

## 📂 Project Structure

```
📁 Customer-Behavior-Analysis
│── 📄 CUSTOMER_BEHAVIOUR_ANALYSIS_SQL.sql
│── 📄 CUSTOMER SHOPING BEHAVIOUR.ipynb
│── 📊 Customer_Behavior_Dashboard.pbix
│── 📄 Final Report Premium.pdf
│── 📄 README.md
```

---

## 🧹 Data Cleaning (Python)

* Removed duplicate records
* Handled missing values
* Standardized categorical values (Yes/No)
* Converted data types
* Feature engineering for better insights

---

## 📊 Exploratory Data Analysis (EDA)

Key analysis performed:

* Revenue by category
* Gender-based purchasing behavior
* Discount impact on purchase value
* Subscription vs non-subscription comparison
* Age group analysis

📌 **Key Finding:**
Few categories contribute to majority of revenue (Pareto pattern).

---

## 💾 SQL Business Analysis

### 🔥 Key Business Questions Solved:

* Which category generates highest revenue?
* Do discounts increase purchase value?
* Do subscribed customers spend more?
* Top 5 products by rating?
* Customer segmentation (New / Returning / Loyal)
* Top products within each category (using window functions)

📌 Advanced Concepts Used:

* Aggregations (SUM, AVG)
* CASE statements
* Subqueries
* Window Functions (`RANK()`)

---

## 📈 Power BI Dashboard
<img width="1920" height="1080" alt="Screenshot (98)" src="https://github.com/user-attachments/assets/65be2e3b-a540-4c2d-83e0-80e12686825d" />
<img width="1920" height="1080" alt="Screenshot (99)" src="https://github.com/user-attachments/assets/35c0f692-aa60-4a29-9218-82169556c979" />

### Dashboard Features:

* KPI Cards (Revenue, Avg Purchase, Customers)
* Interactive Filters (Category, Gender, Subscription)
* Visuals:

  * Revenue by Category
  * Customer Segmentation
  * Discount Impact
  * Age Group Analysis

---

## ⚡ DAX Measures

```DAX
Total Revenue = SUM(customer_behaviour[purchase_amount])

Avg Purchase = AVERAGE(customer_behaviour[purchase_amount])

Customer Count = DISTINCTCOUNT(customer_behaviour[customer_id])

Discount % = 
DIVIDE(
    CALCULATE(COUNT(customer_id), customer_behaviour[discount_applied]="Yes"),
    COUNT(customer_id)
)
```

---

## 🎯 Key Insights

* 🛒 Top categories drive maximum revenue
* 💸 Discounts are not always effective
* 👥 Loyal customers generate high value
* 📦 Express shipping users spend more
* 🔁 Repeat buyers likely to subscribe

---

## 🚀 Business Recommendations

* Focus marketing on high-performing categories
* Introduce loyalty programs
* Optimize discount strategy (targeted offers)
* Promote subscription model
* Improve low-rated products

---

## 🏁 Conclusion

This project showcases:

* End-to-end data analytics workflow
* Strong SQL and data handling skills
* Business-oriented thinking
* Dashboard storytelling

💼 **Perfect for Data Analyst / Business Analyst roles**

---
