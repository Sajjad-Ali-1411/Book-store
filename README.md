
# 📚 Online Bookstore Data Analysis Using SQL

## 📌 Overview

This project demonstrates end-to-end **data analysis of an online bookstore** using SQL. It covers data modeling, importing CSV files into PostgreSQL, and writing queries for business intelligence insights. The project showcases skills in **SQL querying, joins, aggregation, window functions, and real-world data problem-solving**.

---

## 📂 File Structure

- `Books.csv` — Book master data
- `Customers.csv` — Customer records
- `Orders.csv` — Transactional order data
- `bookstore_analysis.sql` — All SQL queries used in analysis
- `README.md` — Project documentation
---

## 🗂️ Dataset Description

The analysis is based on three core tables:

- **Books**: Contains metadata about each book (title, author, genre, price, stock, etc.)
- **Customers**: Stores customer demographic data (name, email, country, etc.)
- **Orders**: Captures order details like order date, quantity, and total amount.

---

## 🛠️ Database Setup

```sql
CREATE DATABASE OnlineBookstore;
```

Tables created:

- `Books`
- `Customers`
- `Orders`

Data is imported using the `COPY` command from CSV files.

---

### 🔍 SQL Analysis Highlights
Includes queries such as:
- Total revenue generation
- Best-selling genres and books
- Customer-wise and city-wise revenue
- Books that are in stock vs. out of stock
- Most active customers and high-value buyers
- Year-wise and genre-wise performance trends

---

### 📊 Key Insights
- **Fiction and Fantasy genres** are the most popular among customers, driving the highest sales volume.
- Some books are **frequently ordered**, while others have **never been purchased**, indicating a skew in demand.
- **Top customers** are contributing a large share of the revenue, with a few individuals spending significantly more than others.
- Revenue is **concentrated in specific years and cities**, suggesting peak times and regional demand.
- Some authors consistently generate **high sales**, making them valuable to stock and promote.
- There's a **significant variance in pricing**, with a few high-priced books and many low/mid-priced ones.
- **Stock management** shows some books running low or sold out, while others are still in high stock.
- Orders with **multiple quantities** are common, suggesting bundled purchasing behavior.

---

### 💡 Business Recommendations
- 📦 **Restock popular titles and authors** promptly to avoid missing sales opportunities.
- 🛍️ Consider **promotions or discounts** on books that are never or rarely ordered to move inventory.
- 📈 Focus marketing campaigns on **Fiction and Fantasy genres**, as they show high engagement.
- 🎯 Launch **loyalty programs** or personalized offers for high-spending customers to retain them.
- 📚 Use genre-wise insights to guide **curation and catalog expansion**.
- 🧮 Adjust procurement strategy based on **stock vs. demand analysis**.
- 🌍 Target marketing efforts in **cities with high spending** and explore why certain regions underperform.
- 🗓️ Monitor **year-over-year sales** to detect trends and plan seasonal campaigns

---

## 🧠 Skills Demonstrated

- SQL Joins (INNER, LEFT)
- Aggregations: `SUM()`, `COUNT()`, `AVG()`
- Filtering and sorting data
- Grouping with `GROUP BY` and `HAVING`
- Window functions: `DENSE_RANK() OVER(...)`
- CTEs (Common Table Expressions)
- Conditional logic with `COALESCE()`

---

## 📈 Sample Business Insights

- 💰 *Total Revenue Generated*: Calculated using SUM on `total_amount`
- 📉 *Books Never Sold*: Identified using LEFT JOIN + IS NULL
- 📊 *Most Popular Genres and Authors*: Based on total units sold
- 🛒 *Top Customer by Spending*: Ranked by total order amount

---

## ✅ Conclusion

This project provides a strong foundation for SQL analysis in real-world business domains like **e-commerce and inventory management**. It demonstrates how SQL can be used not only for querying but also for drawing strategic business insights from structured data.

---

## 🚀 How to Run

1. Clone this repo
2. Load data into PostgreSQL using the provided SQL schema and `COPY` commands
3. Run the SQL queries from `bookstore_analysis.sql` in any SQL editor (e.g., pgAdmin, DBeaver)

---

## 📬 Contact

If you have any feedback, suggestions, or questions, feel free to connect via GitHub Issues or Discussions.
