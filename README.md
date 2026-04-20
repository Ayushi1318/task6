# task6
If you want a more professional version (with charts, graphs, or bigger dataset), tell me and I’ll upgrade it. 
Sales Trend Analysis Using SQL
📌 Project Overview

This project analyzes monthly sales trends using SQL. It focuses on calculating total revenue and order volume from an online sales dataset.

🎯 Objective
Analyze sales performance by month and year
Calculate total revenue using aggregation
Count total orders using distinct values
🛠️ Tools Used
PostgreSQL / MySQL / SQLite
SQL (Structured Query Language)
📂 Project Files
raw_dataset.pdf → Contains sample sales data
sql_code.pdf → SQL script for analysis
output_screenshot.png → Result of executed query
🧠 Concepts Used
GROUP BY for monthly grouping
ORDER BY for sorting results
SUM() for total revenue
COUNT(DISTINCT) for order volume
EXTRACT() for month and year
💻 SQL Query Used
SELECT 
    EXTRACT(YEAR FROM order_date) AS year,
    EXTRACT(MONTH FROM order_date) AS month,
    SUM(amount) AS total_revenue,
    COUNT(DISTINCT order_id) AS total_orders
FROM online_sales
GROUP BY year, month
ORDER BY year, month;
📈 Output

The query returns:

Monthly revenue
Number of orders per month
📚 Learning Outcome
Understanding aggregation functions
Analyzing time-based data
Writing efficient SQL queries
🚀 Conclusion

This project demonstrates how SQL can be used to analyze sales trends and generate meaningful business insights.
