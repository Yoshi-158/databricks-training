# Day 1 - SQL Basic Queries Practice

## Objective
Practice fundamental SQL queries using a simple employee-management database.

The goal of Day 1 is to understand basic SQL operations such as data retrieval, filtering, pattern matching, and date-based querying.

---

## Files in This Folder
- **day1_sql_practice.sql** – Contains table creation, sample data insertion, and SQL practice queries.
- **README.md** – Documentation for Day 1 SQL practice.

---

## Database Tables Used

### 1. Department
Stores department details.

**Columns**
- `department_id` – unique department identifier
- `name` – department name

### 2. Employee
Stores employee information.

**Columns**
- `emp_id` – unique employee identifier
- `name` – employee name
- `age` – employee age
- `salary` – employee salary
- `department_id` – foreign key linked to Department table
- `hire_date` – employee joining date

### 3. Project
Stores project information assigned to departments.

**Columns**
- `project_id` – unique project identifier
- `name` – project name
- `department_id` – foreign key linked to Department table

---

## Sample Data Inserted
The database contains sample records for:
- departments such as **IT**, **HR**, **Finance**, and **Marketing**
- employees with different ages, salaries, departments, and hire dates
- additional edge-case records such as employees without departments
- projects with and without department mapping

---

## SQL Concepts Practiced

### Basic Selection
- Select all records from a table
- Select only specific columns

### Filtering with WHERE
- Retrieve records based on conditions

### Pattern Matching using LIKE
- Search text using wildcard patterns

### Date-Based Filtering
- Retrieve employees based on hire date conditions

---

## Queries Implemented

### Q1
Select all columns from the Employee table.

### Q2
Select only the name and salary columns from the Employee table.

### Q3
Select employees who are older than 30.

### Q4
Select the names of all departments.

### Q5
Select employees who work in the IT department.

### Q6
Select employees whose names start with **'J'**.

### Q7
Select employees whose names end with **'e'**.

### Q8
Select employees whose names contain **'a'**.

### Q9
Select employees whose names are exactly 9 characters long.

### Q10
Select employees whose names have **'o'** as the second character.

### Q11
Select employees hired in the year **2020**.

### Q12
Select employees hired in **January** of any year.

### Q13
Select employees hired before **2019**.

### Q14
Select employees hired on or after **March 1, 2021**.

### Q15
Select employees hired in the last **2 years**.

---

## Key Concepts Demonstrated
- basic `SELECT` statements
- column projection
- conditional filtering using `WHERE`
- pattern matching using `LIKE`
- date filtering using `YEAR()`, `MONTH()`, and date comparison
- working with foreign-key-based tables

---

## Outcome
Day 1 establishes a strong foundation in SQL basics.

This practice covers essential querying techniques that are useful before moving to joins, aggregation, nested queries, and advanced SQL operations.

---

## Notes for Review
- The **Employee** table uses `department_id`, not `department`.
- Date-based query outputs may change depending on the current system date.
- Future aggregation queries can use joins with the **Department** table to display department names instead of IDs.
