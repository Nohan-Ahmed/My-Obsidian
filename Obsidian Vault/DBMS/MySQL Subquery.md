---
source: 
Date created: 2023-11-15
Tagged concepts:
  - MySQL
Type:
  - - tamplate
tags:
  - MySQL
---
A subquery in MySQL is a [[MySQL Queries|query]] nested within another query. It can be used in various parts of a SQL statement, such as the SELECT, FROM, WHERE, or HAVING clauses. Subqueries are enclosed in parentheses and can return a single value, a single row, a single column, or a result set with multiple rows and columns.

>Example:

```MySQL
-- Find students who achieved higher than the average marks
SELECT student_id, f_name, l_name, marks
FROM Student
WHERE marks > (SELECT AVG(marks) FROM Student);

```
#### **Notes:** 
*The inner query executed first gives the result to the outer query, and then the main/outer query will be performed.*
Note: most of the time we use subquery with [[HAVING VS WHERE|WHERE]] clause.