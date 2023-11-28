---
source: 
Date created: 2023-11-16
Tagged concepts: 
Type:
  - - tamplate
---
A Common Table Expression (CTE) is a temporary named যা query result store করতে ব্যবহার হয়।

```MySQL
-- Using a Common Table Expression (CTE)
WITH AverageMarksCTE AS (
    SELECT AVG(marks) AS avg_marks
    FROM Student
)
SELECT student_id, f_name, l_name, marks
FROM Student
WHERE marks > (SELECT avg_marks FROM AverageMarksCTE);
```
