# Some of The Most Important SQL Commands
SELECT - extracts data from a database
UPDATE - updates data in a database
DELETE - deletes data from a database
INSERT INTO - inserts new data into a database
CREATE DATABASE - creates a new database
ALTER DATABASE - modifies a database
CREATE TABLE - creates a new table
ALTER TABLE - modifies a table
DROP TABLE - deletes a table
CREATE INDEX - creates an index (search key)
DROP INDEX - deletes an index

# SQL Select statement

SELECT * FROM table_name;

SELECT column_1, column_2 from table_name;

# The SQL SELECT DISTINCT statement

SELECT DISTINCT column1, column2, ...
FROM table_name;

Example: SELECT DISTINCT Country FROM Customers;

Example With count: SELECT COUNT(DISTINCT Country) FROM Customers;

# SQL WHERE CLAUSE

SELECT column1, column2, ...
FROM table_name
WHERE condition;

Note: The WHERE clause is not only used in SELECT statements, it is also used in UPDATE, DELETE, etc.!

Example: SELECT * FROM Customers
WHERE Country='Mexico';

# Operators in The WHERE Clause
# The following operators can be used in the WHERE clause:

# Refer here in any confusion : https://www.w3schools.com/sql/sql_where.asp
=	Equal	
>	Greater than	
<	Less than	
>=	Greater than or equal	
<=	Less than or equal	
<>	Not equal. Note: In some versions of SQL this operator may be written as !=	
BETWEEN	Between a certain range	
LIKE	Search for a pattern	
IN	To specify multiple possible values for a column

# SQL AND, OR and NOT Operators

# The SQL AND, OR and NOT Operators
The WHERE clause can be combined with AND, OR, and NOT operators.

The AND and OR operators are used to filter records based on more than one condition:

The AND operator displays a record if all the conditions separated by AND are TRUE.
The OR operator displays a record if any of the conditions separated by OR is TRUE.
The NOT operator displays a record if the condition(s) is NOT TRUE.

# AND Syntax

SELECT column1, column2, ...
FROM table_name
WHERE condition1 AND condition2 AND condition3 ...;

Example: SELECT * FROM Customers
WHERE Country='Germany' AND City='Berlin';

# OR Syntax

SELECT column1, column2, ...
FROM table_name
WHERE condition1 OR condition2 OR condition3 ...;

Example: SELECT * FROM Customers
WHERE Country='Germany' OR Country='Spain';

# NOT Syntax

SELECT column1, column2, ...
FROM table_name
WHERE NOT condition;

Example: SELECT * FROM Customers
WHERE NOT Country='Germany';

# Combining AND, OR and NOT

You can also combine the AND, OR and NOT operators.

Example: SELECT * FROM Customers
WHERE Country='Germany' AND (City='Berlin' OR City='München');

Example : SELECT * FROM Customers
WHERE NOT Country='Germany' AND NOT Country='USA';

# SQL ORDER BY Key word

The ORDER BY keyword is used to sort the result-set in ascending or descending order.

The ORDER BY keyword sorts the records in ascending order by default. To sort the records in descending order, use the DESC keyword.

Syntax: SELECT column1, column2, ...
FROM table_name
ORDER BY column1, column2, ... ASC|DESC;

Example: SELECT * FROM Customers
ORDER BY Country;

# ORDER BY DESC

Example: SELECT * FROM Customers ORDER  BY Country, CustomerName;

# SQL LIKE OPERATOR

The LIKE operator is used in a WHERE clause to search for a specified pattern in a column.

There are two wildcards often used in conjunction with the LIKE operator:

 The percent sign (%) represents zero, one, or multiple characters
 The underscore sign (_) represents one, single character

Syntax: SELECT column1, column2, ...
FROM table_name
WHERE columnN LIKE pattern;




| Like Operator                 | Description                                                                  | 
|:-----------------------------:|:----------------------------------------------------------------------------:| 
|WHERE CustomerName LIKE 'a%'   |Finds any values that start with "a"                                          | 
|WHERE CustomerName LIKE '%a'   |Finds any values that end with "a"                                            | 
|WHERE CustomerName LIKE '%or%' |Finds any values that have "or" in any position                               |
|WHERE CustomerName LIKE '_r%'  |Finds any values that have "r" in the second position                         | 
|WHERE CustomerName LIKE 'a_%'  |Finds any values that start with "a" and are at least 2 characters in length  | 
|WHERE CustomerName LIKE 'a__%' |Finds any values that start with "a" and are at least 3 characters in length  |
|WHERE ContactName LIKE 'a%o'   |Finds any values that start with "a" and ends with "o"                        |


Example: SELECT * FROM Customers
WHERE CustomerName LIKE 'a%';





