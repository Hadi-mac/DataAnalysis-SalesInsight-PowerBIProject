# 📊 Sales Insights Data Analysis Project

This project involves analyzing sales data using **MySQL and Power BI**. The data was loaded into a **MySQL local database**, cleaned, transformed, and visualized using an **interactive Power BI dashboard**.

## 📌 Project Overview
- **Data Source**: MySQL database (`db_dump.sql`)
- **Tools Used**: MySQL, Power BI, SQL
- **ETL Process**: Extract, Transform, Load (ETL) from MySQL to Power BI
- **Visualization**: Interactive dashboard for sales insights

## 🚀 How to Set Up the Project
### 1️⃣ Install MySQL and Import the Database
Follow this [tutorial](https://www.youtube.com/watch?v=WuBcTJnIuzo) to install MySQL.

1. Download and install **MySQL Server & MySQL Workbench**.
2. Import the `db_dump.sql` file into MySQL.

### 2️⃣ Run SQL Queries
Here are some sample queries:

-- Show total number of customers
SELECT COUNT(*) FROM customers;

-- Show transactions for Chennai market
SELECT * FROM transactions WHERE market_code = 'Mark001';

-- Show total revenue in 2020
SELECT SUM(transactions.sales_amount) 
FROM transactions 
INNER JOIN date ON transactions.order_date = date.date 
WHERE date.year = 2020;

3️⃣ Load Data into Power BI
Connect Power BI to MySQL using the ODBC connector.
Import tables (customers, transactions, date).
Perform data transformations (normalizing currency, cleaning null values).
Build an interactive dashboard with key insights.

📊 Power BI Dashboard Preview
myProject PowerBI Dashboard Sales Insights.png

🛠 Technologies Used
SQL (MySQL for data extraction and transformation)
Power BI (for visualization and dashboard creation)
ETL Process (Extract, Transform, Load)
Data Cleaning & Transformation (Handling missing values, currency conversion)

📂 Project Files
db_dump.sql - MySQL database dump
myProject PowerBI Dashboard Sales Insights.pbix - Power BI dashboard file
myProject PowerBI Dashboard Sales Insights.png - Dashboard preview
README.md - Project documentation
Sales Analysis PowerBI Dashboard Report.docx - Dashboard Report

📢 Author
Hadi Hussain
