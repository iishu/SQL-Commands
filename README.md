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

Specifies Multiple Conditions Where both 
Of Them Should Be True

SELECT * FROM employees

WHERE department= "IT" AND salary >10000;

## OR
Specifies Multiple Conditions Where Any One
Of Them Should Be True

SELECT * FROM employees;

WHERE department="HR" OR 

department ="FINANCE";

## DISTINCT
Select

Unique Values From A Column

SELECT DISTINCT department FROM employees;

## LIKE
Match A Pattern In A Column

SELECT * FROM employees;

WHERE first_name LIKE "J%";




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

## Aggregate Function
 #  Aggregate functions performs a calculation on a set of values and return a single value.

# COUNT()
# MAX()
# MIN()
# SUM()
# AVG()

SELECT max(marks)

FROM student;


SELECT avg(marks)

FROM student;

## GROUP BY Clause

Groups row s that have the same values into summary rows.
It collects data drom multiple records and groups the result by one or more column.
### Generally we use GROUP BY with some aggregate function.

### Cunt number of students in each city

SELECT city, count(name)
FROM student
GROUP BY city;   

// this will group the names of students with their cities and will give the count of student from each cities

## Query for finding average marks in each city in ascending order

SELECT city, AVG(marks) 

FROM student 

GROUP BY city 

ORDER BY city ASC;


## UPDATE COMMAND

UPDATE student

SET grade="O"



WHERE grade ="A"

###  SET SQL_SAFE_UPDATES=0

//for removing the safe update error

### Cascading Foreign Keys
ON UPDATE CASCADE

ON DELETE CASCADE

#ALTER COMMAND

ADD COLUMN, DROP COLUMN, RENAME TABLE, MODIFY COLUMN

### TRUNCATE COMMANDS

### JOINS SQL

#### INNER JOIN, OUTER JOIN(LEFT JOIN, RIGHT JOIN, FULL JOIN)

### SQL Subquery

SELECT DEPT from employees WHERE  // outer query

salary=(select MAX(salary) from employees);  //inner query

### Practice Question

Name of the employee with max salary in the employee table

SELECT Emp_name from employees WHERE

salary=(select MAX(salary) from employees);


## Triggers

#### It is a user-defined SQL command that is invoked automatically in response to an event such as Insert, Update or Delete.

### Trigger command syntax
CREATE TORGGER
TRIGGER_NAME TRIGGER_TIME
ON TABLE_NAME FOR EACH ROW
BEGIN

.....
END;

### PROCEDURES AND VIEWS IN SQL

#### A SQL View is a virtual table, which is based on SQL SELECT query. A view references one or more existing database tables or other views. It is the snap shot of the database whereas a stored procedure is a group of Transact-SQL statements compiled into a single execution plan.

### UNIONS IN SQL



