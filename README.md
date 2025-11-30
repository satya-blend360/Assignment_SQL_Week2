
# 🛍 Retail Sales Database — Design & Analytics

This project focuses on converting an Amazon retail sales dataset into a **normalized relational database** and performing **analytical SQL queries** to uncover business insights.

---

## 🎯 Project Objectives

- Convert cleaned retail dataset into a **relational database schema**
- Normalize data into **3rd Normal Form (3NF)**
- Execute analytical SQL queries for sales insights
- Generate ER diagram & supporting visuals

---

## 🗂 Folder Contents

| File Name | Description |
|----------|-------------|
| **Amazon Sale Report.csv** | Original raw dataset |
| **Cleaned_Amazon_Sale_Report.csv** | Cleaned and preprocessed dataset (used for database loading) |
| **sales.db** | Final SQLite database containing normalized 3NF tables |
| **sql_queries.ipynb** | Jupyter Notebook with: <br>✔ Table creation scripts <br>✔ Data insertion <br>✔ Analytical SQL queries <br>✔ Validation outputs |
| **ER Diagram.png** | Entity Relationship Diagram of the database |
| **Query1.jpg** | Screenshot: Top-selling products by month |
| **Query2.jpg** | Screenshot: Sales by region (JOIN + GROUP BY) |
| **Query3.jpg** | Screenshot: Customers with spend > ₹5000 |

---

## 🧱 Database Design (3NF)

Normalized tables created:
- **Customers**
- **Products**
- **Orders**
- **OrderDetails**

Ensures:
✔ No duplicate customer/product details  
✔ Referential integrity enforced via **Primary/Foreign Keys**  
✔ Scalable & efficient analytical querying  

---

## 🧩 ER Diagram

> Full ERD available in `ER Diagram.png`

Tables & relationships:
```

Customers 1 ────∞ Orders 1 ────∞ OrderDetails ∞──── 1 Products

```

---

## 📊 Analytical SQL Queries

✔ Top-selling product by month  
✔ Sales by region using JOIN + GROUP BY  
✔ Customers with total spend > threshold using HAVING clause  

Results are available as screenshots:
- `Query1.jpg`
- `Query2.jpg`
- `Query3.jpg`

---

## 🔍 Tools & Technologies Used

| Component | Technology |
|----------|------------|
| Database | SQLite |
| Querying | SQL |
| Processing | Python + Pandas |
| Visualization | Built-in Jupyter screenshot capture |

---

## 📈 Key Insights

- Product sales volumes peak in specific months for top categories
- Maharashtra & Karnataka lead in total order revenue
- High-value repeat customers generate majority of profit

These insights can support targeted promotions and stock planning.

---

## 🚀 How to Review the Project

1. Open `sql_queries.ipynb` to view database creation and query execution
2. Explore `sales.db` using any SQLite viewer (DBeaver, DB Browser)
3. View `ER Diagram.png` and screenshots for query evidence

---
