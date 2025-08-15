# 📊 Meesho E-commerce Analytics Dashboard

![Dashboard Screenshot](Screenshot%202025-08-09%20174931.png)

## 📌 Project Overview
This project is a comprehensive **business analysis dashboard** created in **Power BI** to provide data-driven insights into an e-commerce marketplace. The goal was to transform **raw transactional data** into actionable business intelligence for a fictional e-commerce company, **"Meesho"**.

It demonstrates a **full data analytics workflow** — from **data cleaning and transformation** to **exploratory data analysis (EDA)**, visualization, and insight generation.

---

## 🛠 Tools & Technologies
- **Data Preparation:** Python (Pandas)
- **Database:** PostgreSQL
- **Business Intelligence:** Power BI Desktop
- **Version Control:** Git & GitHub

---

## 🔍 Mini EDA Summary
Before building the dashboard, I conducted **Exploratory Data Analysis (EDA)** to understand the dataset and detect potential issues:

1. **Dataset Overview**
   - Total records: ~100k transactions from multiple CSV files.
   - Columns included order details, customer info, payment data, and product categories.

2. **Data Quality Checks**
   - **Missing Values:** Found nulls in `order_approved_date` (~2%) and `customer_zip_code` (~1%).
   - **Duplicates:** No exact duplicates, but some customers had multiple IDs due to registration errors.
   - **Outliers:** Extremely high-order values (> $5,000) — flagged for further review.

3. **Data Distributions**
   - Order value: right-skewed, with most orders between $50–$300.
   - Payment type: dominated by `credit_card` (~58%) and `boleto` (~34%).
   - Category frequency: top categories were `health_beauty`, `watches_gifts`, and `bed_bath_table`.

4. **Initial Trends**
   - Monthly sales peaked mid-2017, followed by a steady decline.
   - Low repeat purchase rate detected (~3%).

These insights shaped the cleaning process (null handling, type corrections, outlier flagging) and guided the dashboard’s KPIs and visualizations.

---

## 📈 Methodology
The project followed a structured workflow:

1. **Data Cleaning & Merging**
   - Cleaned raw e-commerce datasets using Python (Pandas).
   - Merged multiple CSV files into a single dataset.
   - Corrected data types for accurate analysis.

2. **Data Loading**
   - Loaded cleaned data into **PostgreSQL**.
   - Managed datasets using SQL for optimized querying.

3. **Data Modeling & Analysis**
   - Created KPIs using **DAX** in Power BI:
     - Total Sales
     - Total Customers
     - Repeat Customer Ratio

4. **Dashboard Development**
   - Built an **interactive dashboard** in Power BI.
   - Included key charts for sales trends, product performance, and payment preferences.

5. **Insights & Recommendations**
   - Used the dashboard to identify business trends and suggest strategies.

---

## 🔍 Key Insights & Findings
- **Sales Performance:** Total Sales of **13.81M**. Monthly sales trend shows a **decline starting in late 2017**.
- **Customer Retention:** Repeat Customer Ratio is **3.00%**, indicating a **need for loyalty programs** and targeted marketing.
- **Product Performance:** Top-selling categories are `health_beauty`, `watches_gifts`, and `bed_bath_table`.
- **Payment Preferences:** Majority of orders via **credit card** and **boleto** — useful for payment gateway strategies.

---

## 📂 Repository Structure

Dashboard/

│-- data/ # Raw & cleaned datasets

│-- scripts/ # Python data cleaning scripts

│-- dashboard.pbix # Power BI dashboard file

│-- README.md # Project documentation

Load the dashboard.pbix file in Power BI Desktop.

Connect to the provided PostgreSQL database or CSV data for refresh.

---

## 🚀 How to Use
1. Clone this repository:
   ```bash
   git clone https://github.com/Dipanshu7777/Dashboard.git


📢 Future Improvements

Add cohort analysis for customer retention.

Implement automated data cleaning pipelines.

Include advanced segmentation (RFM analysis) in Power BI.
