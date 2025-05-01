# task-7-sales-summary
📊 Task 7 – Basic Sales Summary with Python & SQLite
This project completes Task 7 of the Data Analyst Internship, which involves connecting to an SQLite database, executing SQL queries, summarizing sales data, and visualizing the results in Python.

✅ Objectives
Connect Python to an SQLite database (sales_data.db)

Run SQL queries to summarize sales data by product

Load the result into a pandas DataFrame

Visualize revenue using a bar chart with matplotlib

🧰 Tools Used
Python

SQLite (via sqlite3)

pandas

matplotlib

Jupyter Notebook / .py script

🗃️ Dataset
Source: Online Sales Data.csv

Transformed into a SQLite database with a table named sales

Schema: product, quantity, price

🔍 SQL Query Used
sql
Copy
Edit
SELECT product, 
       SUM(quantity) AS total_qty, 
       SUM(quantity * price) AS revenue 
FROM sales 
GROUP BY product;
GROUP BY product summarizes data per product

SUM(quantity * price) calculates revenue

📈 Visualization
Used matplotlib to plot a bar chart of the top 10 products by revenue

Saved chart as output_charts/top_10_sales_chart.png

🧪 Output
A DataFrame showing product-wise sales quantity and revenue

A bar chart showing top-performing products by revenue

📁 Project Structure
Copy
Edit
├── sales_data.db
├── Online Sales Data.csv
├── task7.py
├── output_charts/
│   └── top_10_sales_chart.png
└── README.md
