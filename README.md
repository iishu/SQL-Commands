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
# AND

Combines Multiple Conditions In A WHERE clause

SELECT * FROM employees

WHERE 

department= "IT" AND salary >10000;

## DISTINCT
Select

Unique Values From A Column

SELECT DISTINCT department FROM employees;

## LIKE
Match A Pattern In A Column

SELECT * FROM employees;

WHERE first_name LIKE "J%";

## OR
Specifies Multiple Conditions Where Any One
Of Them Should Be True

SELECT * FROM employees;

WHERE department="HR" OR 

department ="FINANCE";

## WHERE Clause

# Using Operators in WHERE

Arithmetic Operators: +,-,/,*.%

Comparison Operators: =,!=,>,<.>=,<=

Logical Operators: AND, OR , IN BETWEEN , ALL, LIKE, ANY

Bitwise Operators: &, ||

## BTEWEEN OPERATOR

SELECT * FROM student WHERE marks BETWEEN 80 and 90;




