1. All Orders by Bianca
%%sql result <<
SELECT *
FROM Sales
WHERE Customer = 'Bianca'

2. Total Quantity Sold per Product
%%sql result <<
SELECT ProductName, SUM(Quantity) AS total_quantity
FROM Sales
GROUP BY ProductName

3. Quantity Sold in Jan 2024
%%sql result <<
SELECT SUM(Quantity) AS total_quantity
FROM Sales
WHERE OrderDate BETWEEN '2024-01-01' AND '2024-01-31'

4. Average Unit Price
%%sql result <<
SELECT AVG(UnitPrice) AS average_price
FROM Sales

5. Customers With More Than 2 Orders
%%sql result <<
SELECT Customer, COUNT(*) AS order_count
FROM Sales
GROUP BY Customer
HAVING order_count > 2









