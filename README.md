# 📊 Sales Insights Project

This project is a SQL-based data analysis of retail transactions to uncover actionable business insights. The goal is to help decision-makers understand revenue trends, customer behavior, and product performance through SQL queries and structured data exploration.

---

## 📁 Project Structure

Sales-Insights-Project/
├── Sales_Insights_SQL/ # SQL-based analysis
│ ├── transactions.csv
│ ├── customers.csv
│ ├── products.csv
│ └── sales_queries.sql
├── Sales_Insights_Tableau_Visualization/ # Tableau dashboards
│ └── dashboards.twbx
├── README.md

## 🛠️ Tools & Technologies

- **SQL (MySQL/PostgreSQL)** – Data querying and insights
- **Tableau** – Visual dashboards (Phase 2)
- **Excel / CSV** – Raw data storage
- **Git/GitHub** – Version control

---

## 🔍 Key Insights Extracted

- Monthly revenue trends
- Top-selling products
- Returning vs new customers
- Customer segmentation
- Product-category performance

---

## 🚀 How to Run

### 1. Import the Data
- Use MySQL Workbench or DBeaver
- Create a database (e.g., `sales_insights`)
- Import `transactions.csv`, `customers.csv`, and `products.csv`

### 2. Execute SQL Queries
- Open and run `sales_queries.sql` (or your own custom queries)
- Analyze results using aggregation, joins, subqueries, etc.

### 3. (Optional) Visualize in Tableau
- Open `.twbx` file in Tableau Public/Desktop
- Refresh data sources to match your local path

---

## 📈 Sample Query

-- Monthly Revenue Trend
SELECT 
  MONTH(transaction_date) AS month, 
  SUM(amount) AS revenue 
FROM transactions
GROUP BY month
ORDER BY month;


🙌 Credits
Project inspired by Codebasics' Data Analysis projects.
Maintained and extended by Abheesht Mishra.

📄 License
This project is open-source and available under the MIT License.
