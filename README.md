# Sales Summary using SQLite and Python

This project is part of a Data Analyst Internship Task.
It demonstrates how to use SQL inside Python to extract simple sales insights from a small SQLite database, display results using print statements, and visualize revenue using a basic bar chart.

## 📌 Objective

Connect to a SQLite database using Python

Run basic SQL queries to calculate:

Total quantity sold

Total revenue per product

Display results in the console

Visualize revenue using a simple bar chart

## 🛠️ Tools & Technologies

Python

SQLite (via sqlite3)

Pandas

Matplotlib

Jupyter Notebook or .py file

SQLite comes built-in with Python — no additional setup required.

## 📂 Dataset

A small SQLite database named:

sales_data.db
Table: sales
Column	Type	Description
id	INTEGER	Primary key
product	TEXT	Product name
quantity	INTEGER	Quantity sold
price	REAL	Price per unit

## 📁 Project Structure
📦 sales-summary-sqlite
 ┣ 📜 sales_analysis.py   # Python script / notebook
 ┣ 📜 sales_data.db       # SQLite database
 ┣ 📊 sales_chart.png     # Generated bar chart (optional)
 ┗ 📜 README.md           # Project documentation
📈 SQL Query Used
SELECT 
    product,
    SUM(quantity) AS total_qty,
    SUM(quantity * price) AS revenue
FROM sales
GROUP BY product;

## 🚀 How to Run the Project

Clone the repository

git clone https://github.com/your-username/sales-summary-sqlite.git
cd sales-summary-sqlite

Install required libraries

pip install pandas matplotlib

Run the script

python sales_analysis.py

Or open the notebook in Jupyter Notebook and run all cells.

## 📊 Output

Printed summary of total quantity and revenue per product

A bar chart showing revenue by product

Optional saved chart: sales_chart.png

## 📌 Key Learnings

Using SQL queries inside Python

Connecting to SQLite databases

Loading SQL results into Pandas DataFrames

Creating basic visualizations with Matplotlib

## ✅ Deliverables Completed

✔ SQLite database connection

✔ SQL aggregation queries

✔ Console output using print()

✔ Bar chart visualization
