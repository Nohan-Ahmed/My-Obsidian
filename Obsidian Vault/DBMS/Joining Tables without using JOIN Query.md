---
source: 
Date created: 2023-11-16
Tagged concepts: 
Type:
  - - tamplate
---

2 or more tables থাকলে table গুলোর properties এ access করতে dot notation ব্যবহার করা হয়।
> example

```MySQL
SELECT 
    emp.first_name AS Name, dep.department_id AS Department_id
FROM
    employees AS emp,
    departments AS dep
WHERE
    dep.department_id = 90 and emp.department_id = dep.department_id;
```
