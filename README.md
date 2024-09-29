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

## BETWEEN OPERATOR(selects for a given range)

SELECT * FROM student WHERE marks BETWEEN 80 and 90;

## IN operator (matches any value in the list)

SELECT * FROM student WHERE city IN ("DELHI","MUMBAI");

## NOT IN

SELECT * FROM student WHERE city NOT IN ("Delhi");

## LIMIT Clause

It will show data in certin limit

SELECT * FROM student WHERE marks>80

LIMIT 3;

//It will show the data of students whose marks are >80 and will show only the data of 3 students

## ORDER BY Clause

to sort data in ascending(ASC) or descending(DESC)  order

SELECT * FROM student

ORDER BY marks ASC;

this will show the data according to marks in increasing order







