# Task 21: Basic SQL SELECT Queries

## 1. Project Overview
This project focuses on practising basic SQL queries using a sample Customers table in Google Colab. It demonstrates how to retrieve, filter, sort, and summarize customer data using SQL.

## 2. Objective
- Understand the SQL `SELECT` statement.
- Filter records using `WHERE`.
- Sort data using `ORDER BY`.
- Search for patterns using `LIKE`.
- Filter multiple values using `IN`.
- Limit query results using `LIMIT`.
- Group records and count customers using `GROUP BY` and `COUNT()`.

## 3. Tools and Technologies
- Google Colab
- Python
- SQLite
- SQL
- Pandas

## 4. Dataset Description
A sample Customers table was created with five customer records.

| Column | Description |
|---|---|
| CustomerID | Unique customer identification number |
| CustomerName | Name of the customer |
| City | Customer's city |

## 5. SQL Queries, Outputs, and Observations

### Query 1: Display Customer Names and Cities

**SQL Query**
```sql
SELECT CustomerName, City
FROM Customers;
```

**Output**

| CustomerName | City |
|---|---|
| Rahul | Hyderabad |
| Priya | Vijayawada |
| Arjun | Guntur |
| Sneha | Hyderabad |
| Kiran | Chennai |

**Observation:** Displays the name and city of every customer.

### Query 2: Find Customers from Hyderabad

**SQL Query**
```sql
SELECT CustomerName, City
FROM Customers
WHERE City = 'Hyderabad';
```

**Output**

| CustomerName | City |
|---|---|
| Rahul | Hyderabad |
| Sneha | Hyderabad |

**Observation:** Two customers belong to Hyderabad.

### Query 3: Sort Customers Alphabetically

**SQL Query**
```sql
SELECT CustomerName, City
FROM Customers
ORDER BY CustomerName ASC;
```

**Output order:** Arjun, Kiran, Priya, Rahul, Sneha.

**Observation:** Sorts customer names in ascending alphabetical order.

### Query 4: Find Customers from Guntur

**SQL Query**
```sql
SELECT CustomerName, City
FROM Customers
WHERE City = 'Guntur';
```

**Output**

| CustomerName | City |
|---|---|
| Arjun | Guntur |

**Observation:** One customer belongs to Guntur.

### Query 5: Find Names Starting with S

**SQL Query**
```sql
SELECT CustomerName, City
FROM Customers
WHERE CustomerName LIKE 'S%';
```

**Output**

| CustomerName | City |
|---|---|
| Sneha | Hyderabad |

**Observation:** The `LIKE 'S%'` condition finds customer names starting with S.

### Query 6: Sort Customers by City

**SQL Query**
```sql
SELECT CustomerName, City
FROM Customers
ORDER BY City ASC;
```

**Observation:** Sorts customer records by city in ascending alphabetical order.

### Query 7: Sort Names in Descending Order

**SQL Query**
```sql
SELECT CustomerName, City
FROM Customers
ORDER BY CustomerName DESC;
```

**Output order:** Sneha, Rahul, Priya, Kiran, Arjun.

**Observation:** Sorts customer names in reverse alphabetical order.

### Query 8: Find Customers from Hyderabad or Guntur

**SQL Query**
```sql
SELECT CustomerName, City
FROM Customers
WHERE City IN ('Hyderabad', 'Guntur');
```

**Output**

| CustomerName | City |
|---|---|
| Rahul | Hyderabad |
| Arjun | Guntur |
| Sneha | Hyderabad |

**Observation:** The `IN` operator retrieves customers from either specified city.

### Query 9: Display the First Three Customers

**SQL Query**
```sql
SELECT CustomerID, CustomerName, City
FROM Customers
LIMIT 3;
```

**Output**

| CustomerID | CustomerName | City |
|---:|---|---|
| 1 | Rahul | Hyderabad |
| 2 | Priya | Vijayawada |
| 3 | Arjun | Guntur |

**Observation:** The `LIMIT 3` clause returns three records.

### Query 10: Count Customers in Each City

**SQL Query**
```sql
SELECT City, COUNT(*) AS TotalCustomers
FROM Customers
GROUP BY City
ORDER BY TotalCustomers DESC;
```

**Output**

| City | TotalCustomers |
|---|---:|
| Hyderabad | 2 |
| Vijayawada | 1 |
| Guntur | 1 |
| Chennai | 1 |

**Observation:** Hyderabad has the highest number of customers in this sample dataset.

## 6. Methodology
1. Imported SQLite and Pandas in Google Colab.
2. Created an in-memory SQLite database.
3. Created the Customers table.
4. Inserted five sample customer records.
5. Executed 10 SQL queries.
6. Displayed the results using Pandas DataFrames.
7. Analysed the query outputs to understand customer data.

## 7. Key Learnings
- SQL data retrieval using `SELECT`.
- Filtering records using `WHERE`.
- Sorting data using `ORDER BY ASC` and `DESC`.
- Pattern matching using `LIKE`.
- Filtering multiple values using `IN`.
- Limiting results using `LIMIT`.
- Grouping records using `GROUP BY`.
- Counting records using `COUNT()`.

## 8. Conclusion
This task provided practical experience with fundamental SQL commands. It improved my understanding of retrieving, filtering, sorting, and summarizing customer data using SQL in Google Colab.

## 9. Internship Details
- **Organization:** Veda Technology
- **Task:** Task 21 – Basic SQL SELECT Queries
- **Author:** M. Navya Sri

## 10. Note
This project uses sample customer data and SQLite in Google Colab for practice. MySQL and PostgreSQL were listed in the task description but were not used in this notebook.
