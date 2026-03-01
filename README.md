# goit-rdb-hw-05
SQL. Nested queries. Code reuse
# SQL Homework 3 – MySQL Queries and Functions

This repository contains solutions for Homework 3, implemented in **MySQL 8.0.44**. The tasks cover various SQL concepts including **nested subqueries, aggregate functions, CTEs (Common Table Expressions), and user-defined functions**.  

## Contents

1. **Display `order_details` with `customer_id`**  
   - Used a **subquery in the SELECT clause** to fetch the corresponding `customer_id` from the `orders` table for each record in `order_details`.

2. **Filter `order_details` by `shipper_id = 3`**  
   - Applied a **subquery in the WHERE clause** to filter only the orders assigned to shipper 3.

3. **Average quantity per order for `quantity > 10`**  
   - Used a **subquery in the FROM clause** to first select records with `quantity > 10` and then calculated the **average quantity grouped by `order_id`**.

4. **CTE (WITH) version of task 3**  
   - Implemented the same query using a **Common Table Expression (CTE)** to demonstrate modern SQL syntax.

5. **User-defined function to divide two numbers**  
   - Created a **MySQL function `new_function(number1 FLOAT, number2 FLOAT)`** to return the result of dividing the first parameter by the second.  
   - Applied this function to the `quantity` field from the `order_details` table as an example.

## How to Use

1. Open **MySQL Workbench** or any MySQL client.  
2. Use the database: `USE hw3;`  
3. Execute each query or the function as needed. For example: `SELECT new_function(10, 2);`

## Notes

- MySQL version: **8.0.44**  
- All queries are written for **MySQL** and may require adjustments for other SQL dialects.  
- The repository demonstrates the usage of:
  - Subqueries (`SELECT`, `WHERE`, `FROM`)  
  - Aggregate functions (`AVG`)  
  - CTE (`WITH`)  
  - User-defined functions (`CREATE FUNCTION`)  
