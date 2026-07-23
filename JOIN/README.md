# Advanced-SQL
Views, Stored Procedures, ACID Transactions, and JOIN Statements

## Views
See file Views_HR_Database_Script.sql \
In SQL, a view is an alternative way of representing data that exists in one or more tables. Just like a real table, it contains rows and columns. The fields in a view are fields from one or more real tables in the database. Though views can be queried like a table, views are dynamic; only the definition of the view is stored, not the data.

## Stored Procedures
See file Stored_Procedures_PETSALE_DATASET.sql \
Stored Procedures in SQL are a type of database object that allow you to encapsulate a series of SQL statements into a single routine. They are stored in the database data dictionary and can be invoked from an application program or from the database command interface. Stored procedures can accept input parameters and return multiple values of output parameters. They can also include control-of-flow constructs such as loops and conditional statements. \
Stored procedures offer several benefits including improved performance, higher productivity, ease of use, and increased scalability. They also provide a mechanism for enforcing business rules and data integrity in the database system.

## ACID Transactions
See file ACID_Transactions_BankAccounts-ShoeShop_Database_Script.sql \
A transaction is simply a sequence of operations performed using one or more SQL statements as a single logical unit of work. A database transaction must be ACID (Atomic, Consistent, Isolated and Durable). The effects of all the SQL statements in a transaction can either be applied to the database using the COMMIT command or undone from the database using the ROLLBACK command. 

In this project, we will utilize some commonly used TCL (Transaction Control Language) commands of SQL through the creation of a stored procedure routine. We will use COMMIT statement, which is used to permanently save the changes done in the transactions in a table, and ROLLBACK statement, which is used to undo the transactions that have not been saved in a table. ROLLBACK can only be used to undo the changes in the current unit of work.

## JOIN Statements
SQL JOIN is a clause that combines rows from two or more tables based on a related column between them. The table's relationship is established by comparing the values in the columns. The purpose of using JOINs is to retrieve data from multiple tables in a single query. There are four types of JOINs in SQL: INNER JOIN, LEFT JOIN, RIGHT JOIN, and FULL OUTER JOIN.

INNER JOIN: Returns only the rows with matching values in both tables.
LEFT JOIN: Returns all the rows from the left table and matching rows from the right table.
RIGHT JOIN: Returns all the rows from the right table and matching rows from the left table.
FULL OUTER JOIN: Returns all the rows when a match in the left or right table.

