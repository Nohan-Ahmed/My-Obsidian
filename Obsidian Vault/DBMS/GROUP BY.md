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
The `GROUP BY` statement groups rows that have the same values into summary rows, like "find the number of customers in each country".

The `GROUP BY` statement is often used with [[Aggregate Function|aggregate functions]] (`COUNT()`, `MAX()`, `MIN()`, `SUM()`, `AVG()`) to group the result-set by one or more columns.
### syntax:

```mysql
SELECT _column_name(s)_  
FROM _table_name_  
WHERE _condition_  
GROUP BY _column_name(s)  
_ORDER BY _column_name(s);_

```

### Example

```mysql
SELECT COUNT(CustomerID), Country  
FROM Customers  
GROUP BY Country;
```

The following SQL statement lists the number of customers in each country: