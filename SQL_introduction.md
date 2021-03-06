# Description of SQL

SQL stands for Structure Query Language.  
SQL is a standard language for accessing anfd manipulating databases.  
SQL became a standard of the American National Standards Institute (ANSI) in 1986, and of the International Organization for   Standardization (ISO) in 1987.

# What can SQL Do?

SQL can execute queries against a database  
SQL can retrieve data from a database  
SQL can insert records in a database  
SQL can update records in a database  
SQL can delete records from a database  
SQL can create new databases  
SQL can create new tables in a database  
SQL can create stored procedures in a database  
SQL can create views in a database  
SQL can set permissions on tables, procedures, and views.  


# SQL is a Standard - BUT....
Although SQL is an ANSI/ISO standard, there are different versions of the SQL language.  

However, to be compliant with the ANSI standard, they all support at least the major commands (such as SELECT, UPDATE,  
DELETE, INSERT, WHERE) in a similar manner.  

Note: Most of the SQL database programs also have their own proprietary extensions in addition to the SQL standard!  

# Using SQL in Your Web Site
To build a web site that shows data from a database, you will need:  

An RDBMS database program (i.e. MS Access, SQL Server, MySQL)  
To use a server-side scripting language, like PHP or ASP(In our case it is PHP)  
To use SQL to get the data you want  
To use HTML / CSS to style the page or any Frontend to visualize the data.  

# RDBMS
RDBMS stands for Relational Database Management System.  

RDBMS is the basis for SQL, and for all modern database systems such as MS SQL Server, IBM DB2, Oracle, MySQL, and Microsoft Access.  

The data in RDBMS is stored in database objects called tables. A table is a collection of related data entries and it consists of   columns and rows.  

# Database Tables
A database most often contains one or more tables. Each table is identified by a name (e.g. "Customers" or "Orders"). Tables contain   records (rows) with data.  

# SQL statements

SQL Statements
Most of the actions you need to perform on a database are done with SQL statements.  

The following SQL statement selects all the records in the "Customers" table:  

SELECT * FROM Customers;  

# Keep in Mind That...
SQL keywords are NOT case sensitive: select is the same as SELECT.  

# Semicolon after SQL Statements?
Some database systems require a semicolon at the end of each SQL statement.  

Semicolon is the standard way to separate each SQL statement in database systems that allow more than one SQL statement to be   executed   in the same call to the server.  

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







