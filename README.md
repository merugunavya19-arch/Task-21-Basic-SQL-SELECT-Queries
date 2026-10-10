# Basic SQL SELECT Queries

## Project Overview
This project demonstrates basic SQL operations using a sample Customers table in Google Colab. It focuses on retrieving data, filtering records, sorting results, and grouping customers using SQL queries.

## Objective
- Understand the SQL `SELECT` statement.
- Filter records using `WHERE`.
- Sort data using `ORDER BY`.
- Search for matching text using `LIKE`.
- Filter multiple values using `IN`.
- Limit the number of returned rows using `LIMIT`.
- Count and group customers by city.

## Tools Used
- Google Colab
- Python
- SQLite
- SQL
- Pandas

## Dataset Description
A sample Customers table was created with five records.

**Columns:**
- `CustomerID` – Unique identifier for each customer
- `CustomerName` – Customer name
- `City` – Customer's city

**Cities included:** Hyderabad, Vijayawada, Guntur, and Chennai.

## SQL Queries Implemented
1. Display customer names and cities using `SELECT`.
2. Find customers from Hyderabad using `WHERE`.
3. Sort customer names alphabetically using `ORDER BY ASC`.
4. Find customers from Guntur.
5. Find customer names starting with the letter S using `LIKE`.
6. Sort customers by city.
7. Sort customer names in descending order using `DESC`.
8. Find customers from Hyderabad or Guntur using `IN`.
9. Display the first three customers using `LIMIT`.
10. Count customers in each city using `COUNT()` and `GROUP BY`.

## Methodology
1. Imported SQLite and Pandas in Google Colab.
2. Created an in-memory SQLite database.
3. Created the Customers table.
4. Inserted five sample customer records.
5. Executed SQL queries to retrieve, filter, sort, and group data.
6. Displayed the query results using Pandas DataFrames.

## Key Learnings
- Writing basic SQL queries.
- Selecting specific columns from a table.
- Filtering records based on conditions.
- Sorting query results in ascending and descending order.
- Using `LIKE`, `IN`, and `LIMIT`.
- Grouping data and calculating counts.

## Conclusion
This task helped strengthen my understanding of basic SQL queries and data retrieval. It provided practical experience using SQL with SQLite in Google Colab and demonstrated how queries can organize and summarize customer data.

## Internship Details
**Organization:** Veda Technology  
**Task:** Basic SQL SELECT Queries  
**Author:** M. Navya Sri

## Note
The project uses sample customer data and SQLite in Google Colab for practice. The internship task also mentions MySQL and PostgreSQL; those systems have not been used in this notebook.
