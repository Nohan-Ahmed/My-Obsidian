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

The ALTER TABLE statement is used to alter the structure of a table. It allows to set constraints, modify and delete existing table columns.

##### `ALTER TABLE` statements
- **ADD:** Adds a new column to the table.
- **MODIFY:** Modifies an existing column in the table.
- **DROP:** Deletes a column from the table.
- **RENAME:** Renames a column in the table.
- **ADD CONSTRAINT:** Adds a constraint to the table.
- **DROP CONSTRAINT:** Drops a constraint from the table.
- **DISABLE KEY:** Disables a key on the table.
- **ENABLE KEY:** Enables a key on the table.
- **CHECK:** Checks the syntax of a constraint.

```MySQL
-- Add a new column:
ALTER TABLE customers
ADD email VARCHAR(255) NOT NULL;

-- Modify the data type of a column
ALTER TABLE customers
MODIFY COLUMN age INT;

-- Delete a column:
ALTER TABLE customers
DROP COLUMN last_name;

```

## Update, delete VS Alter, Drop

UPDATE, DELETE statements are used to change the data in the table. অন্য দিকে Alter, Drop statements use করা হয় table এর structural change করার জন্য। মানে table এ নতুন column add কর, existing column delete করা,  Change Data Type ext.


[Tutorial link](https://www.w3schools.com/MySQL/mysql_alter.asp)


