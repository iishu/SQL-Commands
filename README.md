# SQL-Commands

## Querying Data in SQL
SELECT
Retrieve Data From One Or More Tables

SELECT *  FROM employees;

## Filtering Data in SQL
WHERE
Filter Rows Based On Specified Conditions

SELECT * FROM employees
WHERE 
department= "IT"

## SQL Operator
AND
Combines Multiple Conditions In A WHERE clause

SELECT * FROM employees
WHERE 
department= "IT" AND salary >10000;

## DISTINCT
Select Unique Values From A Column

SELECT DISTINCT department FROM employees;

## LIKE
Match A Pattern In A Column
SELECT * FROM employees;
WHERE first_name LIKE "J%";
