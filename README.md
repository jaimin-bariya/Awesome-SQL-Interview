# Awesome-SQL-Interview


# SQL Query & Interview Questions Repository

This repository contains a collection of **SQL queries** and **interview questions** commonly asked in technical interviews. The questions are categorized based on their difficulty levels and cover a wide range of SQL concepts, from basic to advanced.

## Table of Contents
- [Introduction](#introduction)
- [prerequisites](#prerequisites)
- [Repository Structure](#repository-structure)
- [Categories of Questions](#categories-of-questions-part---1)
  - [L0: Basic SQL](#l0-basic-sql)
  - [L1: Intermediate SQL](#l1-intermediate-sql)
  - [L2: Advanced SQL](#l2-advanced-sql)
- [Theory - Common Interview Questions](#theory---common-interview-questions)
  - [Basic SQL Theory Questions](#basic-sql-theory-questions)
  - [ntermediate SQL Theory Questions](#intermediate-sql-theory-questions)
  - [Advanced SQL Theory Questions](#advanced-sql-theory-questions)
  - [Additional SQL Theory Questions](#additional-sql-theory-questions)
    - [General SQL Concepts](#general-sql-concepts)
    - [Indexing and Optimization](#indexing-and-optimization)
    - [Transaction Management](#transaction-management)
    - [Advanced SQL Concepts](#advanced-sql-concepts)
    - [Normalization and Design Principles](#normalization-and-design-principles)
    - [Additional Optimization and Performance-Related Questions](#additional-optimization-and-performance-related-questions)
- [Contributing](#contributing)
- [License](#license)

<br/>

## Introduction
This repository serves as a practical guide for learning **SQL** and preparing for **SQL-related interview questions**. The questions range from basic SQL syntax to complex queries involving database optimization, transactions, joins, subqueries, and advanced SQL techniques.

<br/>



## prerequisites
- Before starting with the practice set, you have to download and set mysql sample database "classicmodels", [click here to download](https://www.mysqltutorial.org/wp-content/uploads/2023/10/mysqlsampledatabase.zip)
- Download diagram of classicmodels db - [click here](https://www.mysqltutorial.org/wp-content/uploads/2018/04/MySQL-Sample-Database-Diagram-PDF-A4.pdf)
- For mroe info go to - [mysql](https://www.mysqltutorial.org/getting-started-with-mysql/mysql-sample-database/)


## Repository Structure
- **Part 1**
  - **L0**: Basic SQL queries and concepts.
  - **L1**: Intermediate SQL queries covering joins, aggregation, and subqueries.
  - **L2**: Advanced SQL queries involving performance optimization, window functions, and more complex scenarios.
- **Part 2**
  - Same as Part 1 with different queries.
- **L3**: For Ultra Pro Max Student/Developer 😅
- **Theory**: SQL theory questions including database design, normalization, transactions, indexing, etc.
 
<br/>

## Categories of Questions Part - 1

## L0: Basic SQL
- Questions related to basic SQL commands such as `SELECT`, `INSERT`, `UPDATE`, and `DELETE`.
- Queries related to basic data manipulation and retrieval from simple tables.

### Query Questions:
1. How do you display all columns and rows from the `customers` table?  
2. Write a query to retrieve only the `customerName` and `phone` from the `customers` table.  
3. How do you list all rows where `country` is 'USA' in the `customers` table?  
4. Write a query to find all products in the `products` table with a `buyPrice` less than 50.  
5. How do you fetch all orders with a `status` of 'Shipped' from the `orders` table?  
6. Write a query to display the `productName` and `quantityInStock` for all products in the `products` table.  
7. How do you find the distinct `country` values in the `customers` table?  
8. Write a query to count the total number of customers in the `customers` table.  
9. How do you retrieve all employees whose `jobTitle` is 'Sales Rep'?  
10. Write a query to sort the `products` table by `productName` in ascending order.  
11. How do you fetch the `customerName` and `city` of all customers located in 'Paris'?  
12. Write a query to display the top 10 orders from the `orders` table based on the `orderDate`.  
13. How do you retrieve all `offices` located in the USA?  
14. Write a query to display all employees who work in the office located in 'San Francisco'.  
15. How do you calculate the total number of orders placed in the `orders` table?  
16. Write a query to display the `productName` of all products in the `products` table where `productLine` is 'Classic Cars'.  
17. How do you find the `customerName` of all customers whose `creditLimit` is greater than 50,000?  
18. Write a query to fetch all products that have a `quantityInStock` between 10 and 100.  
19. How do you retrieve all orders placed in the year 2024?  
20. Write a query to display the `employeeNumber` and `firstName` of employees whose last names start with 'B'.  

---
<br/>


## L1: Intermediate SQL
- Queries that involve working with multiple tables, using `JOIN`, `GROUP BY`, `HAVING`, and complex `WHERE` conditions.
- Introduction to subqueries, aggregate functions, and case statements.

### Questions:
1. Write a query to retrieve the `customerName` and `city` for customers in 'USA' and 'France'.  
2. How do you fetch the `employeeNumber`, `lastName`, and `officeCode` of all employees who work in the 'San Francisco' office?  
3. Write a query to find the total number of orders for each customer using `orders` and `customers` tables.  
4. How do you retrieve the `productName`, `quantityInStock`, and `buyPrice` for products that have been ordered more than 10 times?  
5. Write a query to fetch the `orderNumber`, `status`, and `customerName` for orders placed by a customer whose `customerNumber` is 103.  
6. Write a query to find the total sales value (`quantityOrdered * priceEach`) for each order in the `orderdetails` table.  
7. How do you find the average `quantityOrdered` for each `orderNumber` in the `orderdetails` table?  
8. Write a query to list the `productLine` with the highest total revenue (`quantityOrdered * priceEach`) in the `orderdetails` table.  
9. Write a query to display the `employeeNumber`, `firstName`, `lastName`, and the office name where the employee works by joining the `employees` and `offices` tables.  
10. How do you find the customers who have never placed an order?  
11. Write a query to retrieve the `customerName` and the total number of orders placed by each customer (include customers who haven’t placed any orders).  
12. Write a query to find the `productName` and `quantityOrdered` for all orders where the quantity of the product ordered is greater than 50.  
13. How do you retrieve the `employeeNumber`, `firstName`, and the `orderNumber` of employees who have processed an order?  
14. Write a query to calculate the average price of products in the `products` table based on `buyPrice`.  
15. How do you fetch the top 3 most expensive products in the `products` table?  
16. Write a query to retrieve the `customerName`, `orderNumber`, and `orderDate` of all orders that have a status of 'Shipped'.  
17. How do you display the total number of products sold for each `productLine`?  
18. Write a query to find employees who report directly to the employee with `employeeNumber = 1143`.  
19. Write a query to calculate the total number of orders in the `orders` table, grouped by `status`.  
20. How do you find the employees who have the highest `salary` in each office?  

---

<br/>


## L2: Advanced SQL

- Complex SQL queries including **window functions**, **common table expressions (CTEs)**, **transactions**, **stored procedures**, and **optimization techniques**.
- In-depth questions on database performance, indexing, normalization, and advanced joins.

### Questions:
1. Write a query to find the `employeeNumber` and `totalRevenue` (sum of `quantityOrdered * priceEach`) for each employee who processed orders in 2024.  
2. How do you retrieve the `customerName` and `orderNumber` of customers who placed orders in both 2023 and 2024?  
3. Write a query to calculate the `rank` of employees based on their `salary` within each office, using a window function.  
4. How do you find the top 3 products in each `productLine` based on total sales (`quantityOrdered * priceEach`)?  
5. Write a query to find the `productName` and the total quantity ordered for each product where the product has been ordered more than 5 times in the last 6 months.  
6. How do you find the `customerName` and the `total number of orders` for each customer who placed orders worth more than $10,000?  
7. Write a query to display the `employeeNumber`, `firstName`, `lastName`, and their total orders value using a window function (include all employees).  
8. Write a query to calculate the average `orderValue` for each `productLine` (orderValue is the sum of `quantityOrdered * priceEach`).  
9. How do you find the employees who have processed more than 10 orders and have the highest total order value within their office?  
10. Write a query to find the `productName` and the `total revenue generated` by each product in the `orderdetails` table, sorted in descending order.  
11. How do you find customers who have never placed an order and list them alongside their `customerNumber`?  
12. Write a query to calculate the difference between the first and last `orderDate` for each customer.  
13. How do you display the cumulative sum of `quantityOrdered` for each order, ordered by `orderDate`?  
14. Write a query to find the `employeeNumber` and their rank based on the total number of orders they have processed, using `RANK()` or `DENSE_RANK()` window function.  
15. Write a query to find the product(s) that have been ordered in every single order in the `orders` table.  
16. How do you calculate the total revenue from all orders processed by employees from the 'Boston' office in the last quarter?  
17. Write a query to display the highest `orderNumber` for each `customerNumber` and the total revenue for each customer (use subqueries or joins).  
18. How do you calculate the running total of `orderValue` for all orders placed after '2024-01-01' using a window function?  
19. Write a query to find the employee who has processed the most revenue, and display their `employeeNumber`, `firstName`, and `lastName`.  
20. How do you retrieve the `employeeNumber` and their corresponding office with the highest number of orders? Display it alongside the total number of orders processed by each employee.
---

<br/>
<br/>



## Categories of Questions Part - 2

## L0: Basic SQL
- Questions related to basic SQL commands such as `SELECT`, `INSERT`, `UPDATE`, and `DELETE`.
- Queries related to basic data manipulation and retrieval from simple tables.

### Query Questions:
1. Write a query to get all columns from the `employees` table.
2. Write a query to retrieve the `customerName` and `contactLastName` for all customers in the `customers` table.
3. Write a query to find the `productName` and `buyPrice` for all products.
4. Write a query to retrieve the `employeeNumber` and `lastName` for employees who have an `officeCode` of '1'.
5. Write a query to list the `orderNumber` and `orderDate` for all orders made in the year 2023.
6. Write a query to find the `customerName` and `phone` of customers whose `contactFirstName` is 'John'.
7. Write a query to retrieve the `productCode` and `productName` for products that have `quantityInStock` less than 50.
8. Write a query to fetch the `orderNumber`, `status`, and `orderDate` of orders placed by customer `customerNumber = 102`.
9. Write a query to get the `customerName` and `city` for customers located in 'Paris'.
10. Write a query to list all employees and their corresponding `jobTitle` from the `employees` table.
11. Write a query to retrieve the `productName` and `buyPrice` for products whose price is greater than $30.
12. Write a query to get the `orderNumber` and `shippedDate` of orders that were shipped after '2024-01-01'.
13. Write a query to list the `employeeNumber`, `lastName`, and `firstName` of all employees who report to `employeeNumber = 1143`.
14. Write a query to get the total number of products listed in the `products` table.
15. Write a query to display the `productName` and `quantityInStock` for all products in the 'Classic Cars' product line.
16. Write a query to fetch the `productName`, `buyPrice`, and `MSRP` for all products with `buyPrice` greater than `MSRP`.
17. Write a query to find all employees with the job title 'Sales Manager'.
18. Write a query to list the `orderNumber` and `status` for orders placed by `customerNumber = 103` that have been shipped.
19. Write a query to get the `orderNumber` and `orderDate` for orders that are marked as 'Shipped' in the `orders` table.
20. Write a query to find the `employeeNumber` and `lastName` for employees who do not have a manager (`reportsTo` is NULL).

---

<br/>


## L1: Intermediate SQL
- Queries that involve working with multiple tables, using `JOIN`, `GROUP BY`, `HAVING`, and complex `WHERE` conditions.
- Introduction to subqueries, aggregate functions, and case statements.

### Questions:
1. Write a query to find the `customerName`, `employeeNumber`, and `orderNumber` for all orders placed by `customerNumber = 1001`.
2. How do you retrieve the `productName`, `quantityInStock`, and `buyPrice` for products in the `Classic Cars` product line, with quantity more than 10?
3. Write a query to display the `employeeNumber` and `total revenue` generated by each employee (total revenue is `quantityOrdered * priceEach`).
4. Write a query to calculate the average `orderValue` (`quantityOrdered * priceEach`) for each order in the `orderdetails` table.
5. Write a query to retrieve the `customerName` and `total number of orders` for each customer who has placed at least 3 orders.
6. How do you find the `employeeNumber`, `firstName`, and the total `salary` for each employee in the `employees` table?
7. Write a query to find the total sales revenue (`quantityOrdered * priceEach`) for each `productLine`.
8. Write a query to retrieve the `productName`, `buyPrice`, and `MSRP` for products where the price is higher than the average `MSRP` of all products.
9. Write a query to find the `customerName` and the `total revenue` for each customer (`total revenue` is the sum of `quantityOrdered * priceEach`).
10. Write a query to find the total number of orders placed by customers from the 'USA' using the `orders` and `customers` tables.
11. How do you retrieve the list of employees working in the 'San Francisco' office? List their `employeeNumber`, `firstName`, and `lastName`.
12. Write a query to retrieve the `productLine` with the highest total revenue (based on `quantityOrdered * priceEach`).
13. Write a query to find the `orderNumber`, `orderDate`, and the total `orderValue` for each order in the `orders` table.
14. Write a query to list all customers from 'USA' who have placed orders after '2024-01-01'.
15. How do you find the employee with the highest `salary` in each office, and display their `employeeNumber`, `firstName`, and `lastName`?
16. Write a query to find the total number of orders placed by each customer using `orders` and `customers` tables.
17. Write a query to calculate the total sales amount (`quantityOrdered * priceEach`) by each `productCode` from the `orderdetails` table.
18. Write a query to get the `productCode` and total revenue for each product where the total revenue exceeds $1000.
19. How do you retrieve the `employeeNumber` and `total revenue` for each employee who has processed orders worth over $10,000?
20. Write a query to find the `orderNumber` and `orderDate` of all orders where the `status` is 'Shipped' and the `shipDate` is in the year 2023.


---
<br/>


## L2: Advanced SQL
- Complex SQL queries including **window functions**, **common table expressions (CTEs)**, **transactions**, **stored procedures**, and **optimization techniques**.
- In-depth questions on database performance, indexing, normalization, and advanced joins.

### Questions:
1. Write a query to calculate the `rank` of products based on total revenue (`quantityOrdered * priceEach`) using a window function and partition by `productLine`.
2. How do you calculate the total revenue (`quantityOrdered * priceEach`) for each employee, and rank them based on the total revenue generated?
3. Write a query to retrieve the `customerName` and `orderNumber` for customers who have placed orders worth more than $5,000 in total.
4. Write a query to calculate the cumulative sum of `quantityOrdered` for each `orderNumber`, ordered by `orderDate`.
5. Write a recursive query to find the hierarchical structure of employees reporting to the employee with `employeeNumber = 1143`.
6. Write a query to calculate the average order value (`quantityOrdered * priceEach`) for each `productLine`, excluding products with a total order value of less than $1,000.
7. Write a query to display the `employeeNumber`, `firstName`, and `total sales` (sum of `quantityOrdered * priceEach`) for each employee using a window function.
8. Write a query to find the `productName` and total revenue for each product, and rank products by revenue within each product line.
9. Write a query to calculate the total revenue (`quantityOrdered * priceEach`) for each `productLine` and `employee`, partitioned by `employeeNumber`.
10. Write a query to find customers who have placed orders in both 2023 and 2024. Display their `customerName` and `orderNumber`.
11. Write a query to calculate the running total of the `orderValue` for each order, ordered by `orderDate`.
12. Write a query to find the `employeeNumber` and their rank based on the total number of orders processed, using the `RANK()` function.
13. Write a query to find all products that were ordered in every order placed in 2024.
14. Write a query to find the employee who processed the highest revenue and display their `employeeNumber`, `firstName`, and `lastName`.
15. Write a query to display the total number of orders placed by customers from each `country`, and order the result by the number of orders.
16. Write a query to calculate the total revenue (`quantityOrdered * priceEach`) for each `productCode` and display only the top 3 products by revenue.
17. How do you find the `employeeNumber` and total revenue generated for each employee who has processed more than 10 orders?
18. Write a query to find the product(s) with the highest total revenue for each product line.
19. Write a query to calculate the average order value per customer, excluding customers who have placed fewer than 3 orders.
20. Write a query to find the total number of orders and total revenue for each product line, grouped by year.

<br/>

---

<br/>



## **L3: Expert Level (Complex Optimization, Recursive Queries, Advanced Data Manipulation)**  
- These are **expert-level** questions designed to challenge your skills with advanced SQL concepts
- including **performance optimization**, **complex joins**, **subqueries**, **recursive queries**, **CTEs with multiple joins**, and **advanced data manipulation techniques**.

### Questions:
1. **Performance Optimization**: Write a query to find the total revenue (`quantityOrdered * priceEach`) for each `productCode` using **indexes** and optimized joins.  
2. **Subqueries**: Write a query to retrieve the `customerName` and `orderNumber` of customers who placed an order where the `orderDate` is later than the most recent order placed by `customerNumber = 103`.  
3. **Recursive Query**: Write a recursive query to find the **hierarchical structure of employees** (manager-subordinate relationship) in the `employees` table, starting with employee `employeeNumber = 1143`.  
4. **CTE with Multiple Joins**: Write a query to calculate the total revenue (`quantityOrdered * priceEach`) for each `productLine`, but only include `products` ordered in the last 6 months. Use a CTE to organize the query.  
5. **Window Function with Partitioning**: Write a query to calculate the **running total of revenue** (`quantityOrdered * priceEach`) for each `productCode` within each `orderDate` partition, sorted by `orderDate`.  
6. **Self-Join**: Write a query to find all employees who report to the same manager and list their `employeeNumber`, `firstName`, and `lastName`.  
7. **Query Optimization**: Write a query to find the top 5 customers who spent the most in total, optimizing the query by indexing appropriate columns and using joins to calculate the total revenue.  
8. **Handling NULLs**: Write a query to find the `customerName` and the `creditLimit` of customers who have not placed any orders (include customers with NULL `customerNumber` in the `orders` table).  
9. **Advanced Aggregation**: Write a query to calculate the **average order value** for each customer, but exclude customers who have placed less than 3 orders.  
10. **Join Multiple Tables**: Write a query to list the `employeeName`, `officeLocation`, and the total value of orders processed by the employee, joining the `employees`, `offices`, and `orders` tables.  
11. **Advanced Subquery**: Write a query to find the `productCode` and the total revenue generated for each product where the total revenue exceeds the average revenue of all products in the `orderdetails` table.  
12. **CTE with Window Functions**: Write a query to display the top 3 employees with the highest total `salary`, but include their total order value (join `employees` and `orders` using a CTE and window function).  
13. **Recursive CTE**: Write a recursive CTE to display the entire hierarchy of the sales representatives and their managers in the `employees` table.  
14. **Multi-Level Aggregation**: Write a query to find the average `salary` for each `jobTitle` in the `employees` table and then calculate the total average `salary` across all job titles.  
15. **Multi-Table Aggregation**: Write a query to find the `productLine` with the highest total revenue from both `orders` and `orderdetails` tables.  
16. **Dynamic Query Generation**: Write a query to dynamically generate the total order value for each `customerNumber`, where the calculation formula (`quantityOrdered * priceEach`) is customizable in the query.  
17. **Dealing with Data Inconsistencies**: Write a query to identify `customers` who have placed orders but have a `NULL` value for `creditLimit`.  
18. **Advanced Join and Grouping**: Write a query to retrieve the `orderNumber`, `orderDate`, and total order value for each order (use `orders` and `orderdetails`), but only include orders with products from a specific `productLine`.  
19. **Data Anomalies Detection**: Write a query to find any discrepancies between the order date (`orderDate`) and the `shippedDate` where the order was not shipped within 5 days of placing the order.  
20. **Query Optimization with Indexing**: Write a query to find the `customerName` and `total orders value` for each customer who placed orders greater than $5,000, optimizing the query performance by suggesting appropriate indexes.

---

### Explanation of Concepts Covered:
1. **Performance Optimization**: Focusing on indexes and optimized joins.
2. **Recursive Queries**: Useful for hierarchical data like employee-manager relationships.
3. **CTEs (Common Table Expressions)**: Organizing complex queries, especially with multiple joins and aggregations.
4. **Window Functions**: Running totals, rankings, etc., with partitioning.
5. **Advanced Joins**: Self-joins, joins across multiple tables.
6. **Subqueries**: Writing nested queries for advanced filtering and calculation.
7. **Handling NULLs**: Dealing with missing data while fetching relevant results.
8. **Data Anomalies**: Identifying inconsistencies and fixing potential issues in business logic.

These expert-level questions will challenge you to think critically about query optimization, complex data retrieval, and efficient handling of large datasets. They will also help you prepare for interviews at top tech companies.

<br/>

---

<br/>

## Theory - Common Interview Questions

some of the most **common SQL theory questions** that are frequently asked in interviews. These questions test your understanding of SQL concepts, queries, optimization, and the relational database model.

### **Basic SQL Theory Questions**

1. **What is SQL?**
   - SQL (Structured Query Language) is a domain-specific language used for managing and manipulating relational databases. It is used to query, update, insert, and delete data from a database.

2. **What are the different types of SQL commands?**
   - **DML (Data Manipulation Language):** `SELECT`, `INSERT`, `UPDATE`, `DELETE`.
   - **DDL (Data Definition Language):** `CREATE`, `ALTER`, `DROP`, `TRUNCATE`.
   - **DCL (Data Control Language):** `GRANT`, `REVOKE`.
   - **TCL (Transaction Control Language):** `COMMIT`, `ROLLBACK`, `SAVEPOINT`.

3. **What is a primary key?**
   - A **primary key** is a unique identifier for a record in a database table. It ensures that each record is unique and not null.

4. **What is a foreign key?**
   - A **foreign key** is a field in one table that uniquely identifies a row of another table. It establishes and enforces a link between the data in two tables.

5. **What is normalization?**
   - **Normalization** is the process of organizing the attributes and tables of a database to minimize redundancy and dependency. It divides large tables into smaller ones and defines relationships between them.

6. **What is denormalization?**
   - **Denormalization** is the process of combining tables to reduce the complexity of queries and increase query performance, often at the cost of additional storage and redundancy.

7. **What are the types of joins in SQL?**
   - **INNER JOIN:** Returns only matching rows from both tables.
   - **LEFT JOIN (or LEFT OUTER JOIN):** Returns all rows from the left table and matched rows from the right table.
   - **RIGHT JOIN (or RIGHT OUTER JOIN):** Returns all rows from the right table and matched rows from the left table.
   - **FULL JOIN (or FULL OUTER JOIN):** Returns all rows when there is a match in either left or right table.
   - **CROSS JOIN:** Returns the Cartesian product of both tables.

8. **What is an index in SQL?**
   - An **index** is a database object that improves the speed of data retrieval operations on a table. It works similarly to an index in a book, allowing faster access to specific rows.

9. **What is a subquery?**
   - A **subquery** is a query nested inside another query. It can be used in `SELECT`, `INSERT`, `UPDATE`, and `DELETE` statements to provide intermediate results for the main query.

10. **What is a view in SQL?**
    - A **view** is a virtual table based on the result set of a SQL query. It does not store data physically but presents the data from one or more tables in a structured way.

---

### **Intermediate SQL Theory Questions**

11. **What is a stored procedure?**
    - A **stored procedure** is a precompiled collection of SQL statements that can be executed as a unit. It can accept parameters and return results, improving performance and reusability.

12. **What is a trigger in SQL?**
    - A **trigger** is a set of SQL statements that automatically execute or fire when a specified event (like `INSERT`, `UPDATE`, `DELETE`) occurs on a table or view.

13. **What is the difference between `WHERE` and `HAVING` clauses?**
    - **WHERE** is used to filter records before aggregation (used in `SELECT`, `UPDATE`, `DELETE`).
    - **HAVING** is used to filter records after aggregation (used with `GROUP BY`).

14. **What is the difference between `DELETE`, `TRUNCATE`, and `DROP`?**
    - **DELETE:** Removes specific rows from a table based on a condition and can be rolled back.
    - **TRUNCATE:** Removes all rows from a table without logging individual row deletions and cannot be rolled back.
    - **DROP:** Deletes a table, its structure, and its data permanently.

15. **What is the difference between `INNER JOIN` and `OUTER JOIN`?**
    - **INNER JOIN** returns only matching rows from both tables.
    - **OUTER JOIN** returns matched rows from both tables, plus unmatched rows from one or both tables (can be `LEFT`, `RIGHT`, or `FULL`).

16. **What are aggregate functions in SQL?**
    - Aggregate functions perform calculations on a set of values and return a single value. Common aggregate functions include `COUNT()`, `SUM()`, `AVG()`, `MIN()`, `MAX()`.

17. **What is a self join?**
    - A **self join** is a join where a table is joined with itself. This is useful for hierarchical or recursive relationships within the same table.

18. **What is a `CASE` statement in SQL?**
    - The **CASE** statement is used to add conditional logic to SQL queries. It is like an IF-ELSE statement that returns specific values based on conditions.

19. **What is the difference between `UNION` and `UNION ALL`?**
    - **UNION** combines the result sets of two or more queries and removes duplicates.
    - **UNION ALL** combines the result sets and keeps all duplicates.

20. **What is a composite key?**
    - A **composite key** is a primary key that consists of two or more columns to uniquely identify a record in a table.

---

### **Advanced SQL Theory Questions**

21. **What is ACID in database systems?**
    - **ACID** stands for Atomicity, Consistency, Isolation, and Durability. It ensures that database transactions are processed reliably and protects against system failures.

22. **What is a transaction in SQL?**
    - A **transaction** is a sequence of SQL operations that are executed as a single unit of work. A transaction must be completed in full, or not at all (i.e., using `COMMIT` or `ROLLBACK`).

23. **What is the difference between `JOIN` and `UNION`?**
    - **JOIN** combines rows from two or more tables based on a related column.
    - **UNION** combines the result sets of two or more queries into a single result set (only returns unique rows).

24. **What is a database normalization form (1NF, 2NF, 3NF, BCNF)?**
    - **1NF (First Normal Form):** Eliminates duplicate columns and ensures atomicity (each column contains unique values).
    - **2NF (Second Normal Form):** Eliminates partial dependencies, where non-key columns depend on only part of the primary key.
    - **3NF (Third Normal Form):** Eliminates transitive dependencies (non-key columns should not depend on other non-key columns).
    - **BCNF (Boyce-Codd Normal Form):** A stricter version of 3NF where every determinant is a candidate key.

25. **What is a deadlock in SQL, and how can it be prevented?**
    - A **deadlock** occurs when two or more transactions are blocked, each waiting for the other to release resources. It can be prevented by using transaction isolation levels and applying proper locking strategies.

26. **What is the difference between `RANK()` and `DENSE_RANK()`?**
    - **RANK()** assigns ranks with gaps when there are ties.
    - **DENSE_RANK()** assigns ranks without gaps, even when there are ties.

27. **What is a `WITH` clause (Common Table Expressions, CTE)?**
    - The **WITH** clause is used to define a temporary result set (CTE) that can be referenced within a `SELECT`, `INSERT`, `UPDATE`, or `DELETE` statement.

28. **What are the different types of indexes in SQL?**
    - **Unique Index:** Ensures that no two rows have the same values in certain columns.
    - **Composite Index:** An index on multiple columns.
    - **Full-Text Index:** Used for text searching.
    - **Clustered Index:** The data is physically ordered on the disk based on the index key.
    - **Non-Clustered Index:** An index that is separate from the data and helps speed up queries.

29. **What is a surrogate key?**
    - A **surrogate key** is an artificial key used to uniquely identify a record, often implemented as an auto-incremented field.

30. **Explain the concept of sharding in databases.**
    - **Sharding** is a technique of horizontally partitioning a large database into smaller, more manageable pieces called **shards**. Each shard is stored on a separate server or cluster.

<br/>

---

## **Additional SQL Theory Questions**

### **General SQL Concepts**

1. **What is a relational database?**
   - A **relational database** is a type of database that stores data in tables (relations). Each table consists of rows and columns, where each row represents a record, and each column represents an attribute of the record.

2. **What are database constraints, and why are they important?**
   - **Constraints** are rules enforced on data in a table to ensure data integrity. Common types of constraints include `NOT NULL`, `UNIQUE`, `CHECK`, `DEFAULT`, `PRIMARY KEY`, and `FOREIGN KEY`.

3. **What is the difference between `CHAR` and `VARCHAR`?**
   - **CHAR** is a fixed-length string data type, while **VARCHAR** is a variable-length string data type. `VARCHAR` uses only as much space as needed, whereas `CHAR` always uses the defined length.

4. **What is referential integrity?**
   - **Referential integrity** ensures that relationships between tables are maintained consistently. It means that foreign keys in a table must correspond to valid primary keys in another table.

5. **Explain the concept of data consistency in a database.**
   - **Data consistency** means that the data stored in a database is accurate, reliable, and follows the defined rules or constraints at all times.

---

### **Indexing and Optimization**

6. **What are the different types of indexing in SQL, and how do they differ?**
   - **Clustered Index:** Data is physically ordered based on the index key.
   - **Non-clustered Index:** A separate structure that points to the data rows, allowing faster access.
   - **Unique Index:** Ensures that no two rows have the same values in the indexed column(s).
   - **Composite Index:** Indexing on multiple columns.

7. **How does SQL Server handle duplicate rows in a query result?**
   - By default, SQL removes duplicate rows in the query result unless the `DISTINCT` keyword is used. The `DISTINCT` keyword eliminates duplicate rows from the output.

8. **What are the potential problems caused by poor indexing?**
   - Poor indexing can result in slow query performance, increased I/O operations, and long query times, especially with large datasets. Too many indexes can also slow down write operations like `INSERT`, `UPDATE`, and `DELETE`.

9. **What is query optimization, and why is it important?**
   - **Query optimization** is the process of improving the efficiency of a query by reducing its execution time. It is important to ensure that the database performs well even with large datasets and complex queries.

10. **What is the difference between a `UNIQUE` constraint and a `PRIMARY KEY`?**
    - Both **UNIQUE** and **PRIMARY KEY** ensure uniqueness, but a **PRIMARY KEY** also implicitly enforces `NOT NULL`. A table can have only one **PRIMARY KEY**, but it can have multiple **UNIQUE** constraints.

---

### **Transaction Management**

11. **What is a rollback, and when is it used?**
    - A **rollback** undoes all changes made by a transaction. It is used in cases of errors or when a transaction violates database rules.

12. **What are the different isolation levels in SQL?**
    - The **isolation levels** define the visibility of changes made by one transaction to other transactions. They are:
      - **READ UNCOMMITTED**
      - **READ COMMITTED**
      - **REPEATABLE READ**
      - **SERIALIZABLE**

13. **What is a deadlock, and how can it be resolved in SQL?**
    - A **deadlock** occurs when two transactions are waiting on each other to release resources, causing a standstill. It can be resolved by using a timeout, retrying the transaction, or implementing proper locking mechanisms.

14. **What is the difference between `COMMIT` and `ROLLBACK`?**
    - **COMMIT** makes all changes made during the transaction permanent. **ROLLBACK** undoes all changes made during the transaction.

15. **What is a transaction log?**
    - A **transaction log** is a record of all the changes made to the database. It ensures that the database can be recovered to a consistent state after a failure.

---

### **Advanced SQL Concepts**

16. **What is a Materialized View?**
    - A **Materialized View** is a physical copy of a query result stored in a table format. Unlike regular views, materialized views store the result of a query for faster access and can be refreshed periodically.

17. **What is a recursive query?**
    - A **recursive query** is a query that refers to itself. In SQL, recursive queries are often implemented using `WITH` clauses (CTEs) to handle hierarchical data, like organizational charts or category structures.

18. **Explain the difference between `RANK()`, `ROW_NUMBER()`, and `DENSE_RANK()`.**
    - **ROW_NUMBER()** assigns a unique number to each row.
    - **RANK()** assigns ranks to rows with gaps if there are ties.
    - **DENSE_RANK()** assigns ranks without gaps, even with ties.

19. **What is a `WITH` clause (Common Table Expressions, CTE), and how is it different from a subquery?**
    - A **CTE** is a temporary result set that is defined within the execution scope of a `SELECT`, `INSERT`, `UPDATE`, or `DELETE` statement. It is more readable and reusable than a subquery, which is nested within a query.

20. **What is the purpose of `EXPLAIN` in SQL?**
    - The `EXPLAIN` statement is used to analyze and display the execution plan of a query. It helps identify performance bottlenecks and optimize queries by showing how the SQL engine will execute them.

---

### **Normalization and Design Principles**

21. **What is the difference between 3NF and BCNF?**
    - **3NF (Third Normal Form)** ensures that there are no transitive dependencies, meaning non-key columns should not depend on other non-key columns. **BCNF (Boyce-Codd Normal Form)** is a stricter version of 3NF, where every determinant must be a candidate key.

22. **What are candidate keys and alternate keys?**
    - **Candidate keys** are columns that can uniquely identify a record. A **primary key** is selected from the candidate keys. **Alternate keys** are the candidate keys not chosen as the primary key.

23. **What is an ER diagram?**
    - An **Entity-Relationship (ER) diagram** is a visual representation of the database structure, showing entities (tables), attributes (columns), and relationships between entities.

24. **What is the difference between `INSERT INTO` and `INSERT`?**
    - There is no difference between `INSERT INTO` and `INSERT` in SQL. Both are used to insert data into a table. The `INTO` keyword is optional.

25. **What are the various types of relationships in database design?**
    - The types of relationships include:
      - **One-to-One (1:1):** Each record in one table is related to one record in another table.
      - **One-to-Many (1:M):** Each record in one table can relate to multiple records in another table.
      - **Many-to-Many (M:M):** Multiple records in one table can relate to multiple records in another table.

---

### **Additional Optimization and Performance-Related Questions**

26. **What is query execution plan?**
    - The **query execution plan** is the strategy that the database query optimizer uses to execute a SQL query. It shows the steps involved in processing the query, including how tables are accessed, joined, and filtered.

27. **What is denormalization, and when would you use it?**
    - **Denormalization** is the process of combining tables to reduce the complexity of queries and improve performance, particularly in cases where read-heavy operations are more common than write operations.

28. **What are window functions, and how are they different from aggregate functions?**
    - **Window functions** perform calculations across a set of table rows that are related to the current row, without collapsing the result set like aggregate functions.

29. **What is sharding in databases, and how does it work?**
    - **Sharding** is a method of partitioning large databases into smaller, more manageable pieces called **shards**, which are stored across different servers to improve performance and scalability.

30. **What is the difference between a `LOCAL` and `GLOBAL` temporary table in SQL?**
    - A **LOCAL temporary table** is visible only to the session that created it and is dropped automatically when the session ends. A **GLOBAL temporary table** is visible to all sessions, but its data is session-specific.


<br/>

---

<br/>

## Contributing

We welcome contributions to this repository! To contribute, please follow these steps:
1. Fork this repository.
2. Create a new branch (`git checkout -b feature/your-feature`).
3. Add your changes or new questions.
4. Commit your changes (`git commit -m 'Add new SQL question'`).
5. Push to the branch (`git push origin feature/your-feature`).
6. Open a pull request.

If you have any suggestions or questions, feel free to open an issue.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## Acknowledgments

- Thanks to all contributors who have shared their knowledge and questions!
- Special thanks to [classicmodels database](https://github.com/johnpapa/classicmodels) for providing sample database queries for practice.


---

[Go to the Top](#awesome-sql-interview)
