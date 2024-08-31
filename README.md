# Documenting my learning of SQL server

First of all let us get things right SQL server is a Relational Database Management System(RDMS) developed by Microsoft and they have tweaked traditional SQL a with few additional features and named as Transactional SQL(T-SQL)

### So what is SQL ?

SQL is query language for interacting with relational database systems (aka Structured Query Language)

---

### Keywords in SQL:

- `SELECT` Used to select columns(attributes)
- `FROM` Used to get values from a specified table
- `AS` Used for aliasing a column name for better naming convention
- `DISTINCT` Used to get unique values from a table without any repetitions
- `TOP()` Used to get top values from a table when we pass a value like TOP(10)
- `TOP(50)` PERCENT Used for get half the results of a table
- `*` Used to get all rows from a table
- `ORDER BY` Used to order the rows when we get the values from the table, by default order of the rows returned are not same
- `ORDER BY age DESC` Used to order by age in descending order
- `ORDER BY age` Used to order by age in ascending order(default)
  <img width="1074" alt="image" src="https://github.com/user-attachments/assets/c7c06685-c3f5-4341-9ae1-dfef8173589e">
- `WHERE` Used to filter values from a table
  ```SQL
  WHERE age > 18
  WHERE age < 18
  WHERE age >= 18
  WHERE age <= 18
  WHERE name = 'Ironman'
  WHERE order_date = '2025-15-08'
  WHERE age <> 18
  WHERE age BETWEEN 20 AND 30; // 20 and 30 are inclusive
  WHERE age NOT BETWEEN 20 AND 30; NOT of about condition
  WHERE age IS NULL;
  WHERE age IS NOT NULL;
  ```
- `IN` Used to check if a value exists in a query like `WHERE name IN ('Rohit','Dhoni','Sachin')`
- `LIKE` Used to get values starting or ending with, contains characters and get values with specific length
  ```SQL
  -- Names starting with 'John'
  WHERE name LIKE 'John%'

  -- Names ending with 'son'
  WHERE name LIKE '%son'

  -- Names containing 'am' anywhere
  WHERE name LIKE '%am%'

  -- Names with exactly 5 characters
  WHERE name LIKE '_____'

  -- Names starting with 'A' and having exactly 5 characters
  WHERE name LIKE 'A____'
  ```
---

### What is NULL value ?

It is used to signify a record that has no value, we can also filter values from a table based null values as shown above






