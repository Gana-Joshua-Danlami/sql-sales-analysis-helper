# 📊 SQL Sales Analysis — Query Explanations

This markdown explains the SQL logic behind each question in the `queries_and_solutions.ipynb` file. The goal is to **help you understand why the queries work**, not just copy them.

---

### Question 1: Retrieve All Orders by Bianca

**SQL:**
```sql
SELECT * FROM Sales WHERE Customer = 'Bianca';
Explanation:

We use SELECT * to fetch all columns from the Sales table.

WHERE Customer = 'Bianca' filters the rows to only include orders made by Bianca.


✅ Question 2: Total Quantities Sold Per Product
SQL:
SELECT ProductName, SUM(Quantity) AS total_quantity
FROM Sales
GROUP BY ProductName;

Explanation:
SUM(Quantity) adds all quantities sold for each product.

GROUP BY ProductName ensures the sum is calculated per product.

The alias total_quantity is required to match test expectations.


✅ Question 3: Total Quantity Sold in January 2024
SQL:
SELECT SUM(Quantity) AS total_quantity
FROM Sales
WHERE OrderDate BETWEEN '2024-01-01' AND '2024-01-31';

Explanation:
BETWEEN filters the date range from Jan 1 to Jan 31.

SUM(Quantity) totals the units sold within that period.


✅ Question 4: Calculate Average Unit Price
SQL:
SELECT AVG(UnitPrice) AS average_price
FROM Sales;

Explanation:
AVG(UnitPrice) calculates the mean price of all items sold.

AS average_price gives the result a readable alias.


✅ Question 5: Customers with More Than 2 Orders
SQL:
SELECT Customer, COUNT(*) AS order_count
FROM Sales
GROUP BY Customer
HAVING COUNT(*) > 2;

Explanation:
GROUP BY Customer groups sales by each customer.

COUNT(*) counts how many orders each customer made.

HAVING COUNT(*) > 2 filters the result to customers with more than two orders.

We use HAVING instead of WHERE because it works with aggregates like COUNT().


Got questions? DM or fork the repo to experiment. Happy learning!






