Day 1 - SQL Basic Queries Practice

Objective
Practice fundamental SQL queries using a simple employee-management database.
The goal is to understand data retrieval, filtering, pattern matching, and date-based querying using basic SQL commands.

Files in This Folder
day1_sql_practice.sql - SQL script containing table creation, sample data insertion, and practice queries
README.md - documentation for Day 1 SQL practice

Database Tables Used

1. Department
Stores department details.

Columns:
department_id - unique department identifier
name - department name

2. Employee
Stores employee information.

Columns:
emp_id - unique employee identifier
name - employee name
age - employee age
salary - employee salary
department_id - foreign key linked to Department table
hire_date - employee joining date

3. Project
Stores project information assigned to departments.

Columns:
project_id - unique project identifier
name - project name
department_id - foreign key linked to Department table

Sample Data Inserted
The dataset contains sample records for:
multiple departments such as IT, HR, Finance, and Marketing
employees with different ages, salaries, departments, and hire dates
additional edge-case records such as employees without departments
projects with and without department mapping

SQL Concepts Practiced

1. Basic Selection
Select all records from a table
Select specific columns only

Queries covered:
select all employee records
select employee name and salary

2. Filtering with WHERE
Retrieve records based on conditions

Queries covered:
employees older than 30
employees working in IT department

3. Pattern Matching using LIKE
Search text using wildcard patterns

Queries covered:
names starting with J
names ending with e
names containing a
names with exactly 9 characters
names having o as the second character

4. Date-Based Filtering
Retrieve employees based on hire date conditions

Queries covered:
employees hired in the year 2020
employees hired in January
employees hired before 2019
employees hired on or after 1 March 2021
employees hired in the last 2 years

Queries Implemented

Q1
Select all columns from Employee table

Q2
Select name and salary from Employee table

Q3
Select employees older than 30

Q4
Select names of all departments

Q5
Select employees in IT department

Q6
Select employees whose names start with J

Q7
Select employees whose names end with e

Q8
Select employees whose names contain a

Q9
Select employees whose names are exactly 9 characters long

Q10
Select employees whose names have o as the second character

Q11
Select employees hired in the year 2020

Q12
Select employees hired in January

Q13
Select employees hired before 2019

Q14
Select employees hired on or after March 1, 2021

Q15
Select employees hired in the last 2 years

Key Concepts Demonstrated
basic SELECT statements
column projection
conditional filtering with WHERE
string filtering using LIKE
date filtering using YEAR(), MONTH(), and date comparison
working with foreign-key-based tables

Outcome
Day 1 builds a strong foundation in SQL basics.
The practice covers core querying techniques that are essential before moving to joins, aggregation, nested queries, and advanced database operations.

Notes for Review
The Employee table uses department_id, not department.
For future aggregation queries, joins with the Department table can be used to display department names instead of department IDs.
The output of date-based queries may change depending on the current system date.
