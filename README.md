# SQL Data Analysis Project: Classic Models Business Insights

## Overview
This project is a detailed SQL analysis of the **Classic Models Database**, a relational dataset representing a fictional company selling classic car models. Using over 40 SQL queries, I explore sales performance, customer behavior, employee contributions, and product trends. The analysis is conducted in a Jupyter Notebook with Python, leveraging `pandas` and `SQLAlchemy` to connect to a MySQL database, execute queries, and process results.

The project demonstrates my SQL proficiency across a wide range of topics—basic queries, joins, aggregations, subqueries, window functions, indexing, stored procedures, triggers, and views—while delivering actionable business insights. It’s designed as a portfolio piece to showcase my data analysis skills.

---

## Dataset
The **Classic Models Database** consists of 8 relational tables:
- **Customers**: Customer details (e.g., ID, name, credit limit, sales rep).
- **Orders**: Order records (e.g., ID, customer ID, date, status).
- **OrderDetails**: Order line items (e.g., order ID, product code, quantity, price).
- **Products**: Product catalog (e.g., code, name, product line, stock).
- **Employees**: Employee info (e.g., ID, name, job title, office).
- **Offices**: Office locations (e.g., code, city, country).
- **Payments**: Payment records (e.g., customer ID, date, amount).
- **ProductLines**: Product categories (e.g., line, description).

### Source
- Downloaded from [MySQL Tutorial](https://www.mysqltutorial.org/mysql-sample-database.aspx) as a `.sql` file and imported into MySQL.

### Schema
Tables are linked via keys (e.g., `customerNumber`, `orderNumber`, `productCode`), enabling complex relational analysis.

---

## Project Objectives
- **Master SQL Techniques**: Apply a full spectrum of SQL skills to a real-world dataset.
- **Derive Insights**: Analyze sales, customer activity, and operational trends.
- **Showcase Skills**: Build a professional, reproducible analysis for my portfolio.

---

## Methodology
### Tools
- **Jupyter Notebook**: Hosts the analysis and documentation.
- **Python**:
  - `pandas`: Data manipulation and visualization.
  - `sqlalchemy`: Connects to MySQL for query execution.
- **MySQL**: Database engine hosting the dataset.

### Approach
1. **Setup**: Imported the `.sql` file into MySQL and connected via `SQLAlchemy`.
2. **Exploration**: Inspected table structures, row counts, and data previews.
3. **Analysis**: Executed 40+ queries to investigate key business questions.
4. **Enhancements**: Added indexes, triggers, stored procedures, and views for efficiency and functionality.

### Analysis Scope
- **Data Quality**: Checked table structures, missing values, and duplicates.
- **Customer Insights**: Analyzed customer counts, payments, order frequency, and inactivity.
- **Sales Performance**: Calculated total revenue, average order value, and top products/product lines.
- **Temporal Trends**: Examined revenue by month and year, plus year-over-year growth.
- **Employee Impact**: Linked sales reps to customer activity.
- **Advanced Analytics**: Ranked customers/products, tracked order statuses, and computed per-customer metrics.

---

## Key Insights
- Identified top-spending customers and best-selling products/product lines.
- Uncovered seasonal revenue patterns and order status distributions.
- Highlighted inactive customers and revenue growth trends.
- Optimized query performance with indexing and summarized data with views.

---

## How to Run
### Prerequisites
- Python 3.x
- Libraries: `pandas`, `sqlalchemy`, `mysql-connector-python` (`pip install pandas sqlalchemy mysql-connector-python`)
- MySQL Server
- Jupyter Notebook (`pip install notebook`)

### Setup
1. Clone the repo: `git clone https://github.com/zeeshan-akram-ds/sql_data_analysis_project.git`
2. Download [Classic Models `.sql`](https://www.mysqltutorial.org/mysql-sample-database.aspx) and import:
   ```bash
   mysql -u username -p classicmodels < classicmodels.sql
3. Update the SQLAlchemy connection string in the notebook (e.g., mysql+mysqlconnector://user:password@localhost/classicmodels).
4. Run sql data analysis project.ipynb in Jupyter Notebook.
### Project Structure
1. sql data analysis project.ipynb: Core notebook with analysis and queries.
2. classicmodels.sql: Database source file (download separately).
### Future Enhancements
  Add visualizations (e.g., revenue trends, top customer charts).
  Implement predictive models for sales forecasting.
  Expand with simulated data for broader analysis.
### Author
Zeeshan Akram.  
GitHub: [zeeshan-akram-ds](https://github.com/zeeshan-akram-ds/sql_data_analysis_project)
