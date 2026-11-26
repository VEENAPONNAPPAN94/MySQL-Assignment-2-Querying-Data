## MySQL Assignment 2 – Querying Data

SQL queries covering data retrieval, filtering, sorting, grouping, aggregation, and table joins on the `employee` database (`departments`, `location`, and `employees` tables)

### What’s Included

* **Basic Querying & Filtering**: Retrieving unique salaries (`DISTINCT`), applying column aliases (`AS` for `Employee_Age` and `Employee_Salary`), filtering records with `WHERE` and logical operators (`salary > 50000` and `hire_date < '2016-01-01'`), and updating missing `designation` values to `'Data Scientist'.
* **Sorting & Limiting**: Ordering records by `department_id` (`ASC`) and `salary` (`DESC`), and restricting results with `LIMIT` to display the first 5 employees hired in 2018.
* **Aggregations & Grouping**: Calculating total Finance department salary (`SUM`) and minimum employee age (`MIN`)[cite: 5], grouping by location for maximum salary (`MAX`) and by `'Analyst'` designations for average salary (`AVG` with `LIKE`), and filtering grouped results using `HAVING` (departments with fewer than 3 employees and locations where female employees have an average age below 30).
* **Joins**: Combining `employees`, `departments`, and `location` tables using `INNER JOIN`, `LEFT JOIN` (including departments with zero employees), and `RIGHT JOIN` (displaying all locations with `NULL` for unassigned employees).

### How to Execute

1. Ensure the `employee` database and constrained tables (`departments`, `location`, `employees`) from Assignment 1 are created
2. Run the DML script (`employee data.sql`) to populate the tables.
3. Execute the queries in **MySQL Workbench** or the **MySQL CLI** (MySQL **8.0+**).
