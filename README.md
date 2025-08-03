# Parks and Recreation Employee Demographics - SQL Queries

This project contains basic SQL queries used to explore and analyze the `employee_demographics` table from the `parks_and_recreation` database.

## 📋 Description

The SQL queries in this file are designed to:
- Retrieve all employee data.
- Select specific columns such as first name, last name, age, gender, and birth date.
- Perform a simple calculation using the `age` column.
- Identify unique values in the `gender` column.

These queries are great for beginners learning how to:
- Use the `SELECT` statement.
- Target specific columns.
- Perform column operations.
- Use `DISTINCT` to remove duplicate values.

## 🗂 Table Used
**Table name:** `employee_demographics`  
**Database:** `parks_and_recreation`

### Expected Columns:
- `first_name`
- `last_name`
- `age`
- `gender`
- `birth_date`

## 💻 Sample Queries

```sql
-- Select all columns
SELECT * FROM parks_and_recreation.employee_demographics;

-- Select specific columns
SELECT first_name FROM parks_and_recreation.employee_demographics;
SELECT last_name FROM parks_and_recreation.employee_demographics;

-- Select multiple specific columns
SELECT age, gender FROM parks_and_recreation.employee_demographics;

-- Retrieve birth dates
SELECT birth_date FROM parks_and_recreation.employee_demographics;

-- Perform a simple calculation
SELECT age, age + 10 FROM parks_and_recreation.employee_demographics;

-- Find unique gender values
SELECT DISTINCT gender FROM parks_and_recreation.employee_demographics;
