**SQL Analytics Exercises Repository**
This repository contains a collection of structured SQL exercises designed to demonstrate practical data analysis skills. The project focuses on querying relational databases to extract insights, solve business problems, and build a strong foundation in SQL for data analytics roles.

**Objectives**
Practice core SQL concepts
Analyze structured datasets using queries
Develop problem-solving skills using real-world scenarios
Prepare for data analyst and business intelligence roles

** Tools & Technologies**

SQL (Databricks SQL / Standard SQL)
Microsoft Excel (for dataset structuring and validation)
GitHub (version control and project documentation)

**Project Overview**

The repository includes a series of SQL queries covering different levels of complexity. Each query is designed to answer specific business questions using datasets such as employee records and sales data.

Key focus areas include:

Data filtering and sorting
Aggregation and grouping
Conditional logic using CASE statements
Data ranking and limiting results
Business-driven query design

**Methodology**
Understanding the Dataset
Reviewed dataset structure (columns, data types, relationships)
Query Development
Wrote SQL queries to answer specific analytical questions
Applied SQL clauses such as:
SELECT
WHERE
ORDER BY
GROUP BY
HAVING
LIMIT
CASE WHEN
Validation & Testing
Executed queries in Databricks
Verified outputs for accuracy
Insight Generation
Interpreted query results to derive meaningful insights
📊 Key SQL Concepts Demonstrated
🔹 Filtering Data

Using WHERE, AND, NOT, and IN to refine datasets

🔹 Sorting Results

Using ORDER BY to organize data (ascending/descending)

🔹 Aggregations

Using functions like:

SUM()
AVG()
COUNT()
🔹 Grouping Data

Using GROUP BY to summarize data by categories

🔹 Conditional Logic

Using CASE WHEN to classify and categorize data

🔹 Advanced Filtering

Using HAVING to filter aggregated results

📈 Example Queries

1. Filtering and Sorting Data

SELECT *
FROM employees
WHERE department NOT IN ('Finance')
  AND salary > 50000
ORDER BY hire_date ASC;

2. Aggregation with GROUP BY

SELECT department,
       AVG(salary) AS avg_salary
FROM employees
GROUP BY department;

3. Conditional Logic with CASE

SELECT student_id,
       days_present * 100.0 / total_days AS attendance_percentage,
       CASE
           WHEN days_present * 100.0 / total_days >= 90 THEN 'Excellent'
           WHEN days_present * 100.0 / total_days BETWEEN 75 AND 89.99 THEN 'Good'
           ELSE 'Needs Improvement'
       END AS attendance_status
FROM attendance;

**💡 Key Learnings**
Improved ability to write efficient SQL queries
Gained experience in transforming raw data into insights
Strengthened understanding of database querying for business use cases

**Future Improvements**
Add more complex joins (INNER, LEFT, RIGHT joins)
Incorporate real-world datasets
Build dashboards using Power BI or Tableau
Optimize queries for performance
