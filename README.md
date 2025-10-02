# Task 7: Basic Sales Summary using SQLite and Python

## Objective
The objective of this task was to use SQL inside Python to pull sales information such as:
- Total quantity sold
- Total revenue per product

The results were displayed using print statements and a bar chart.

---

## Tools Used
- Python (`sqlite3`, `pandas`, `matplotlib`)
- SQLite (built into Python, no setup required)
- Jupyter Notebook / Python script

---

## Steps I Performed
- Created a small SQLite database file **`sales_data.db`** with one table **`sales`** containing `product`, `quantity`, and `price`.  
- Connected to the database using Python’s `sqlite3`.  
- Wrote and executed the SQL query:  

```sql
SELECT product, 
       SUM(quantity) AS total_qty, 
       SUM(quantity * price) AS revenue
FROM sales
GROUP BY product;
```

![WhatsApp Image 2025-10-02 at 21 36 35_4892d764](https://github.com/user-attachments/assets/f3aaa21a-97da-45d0-be99-a7f47b94ec49)
