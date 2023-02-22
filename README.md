# PostgreSQL
Code snippets from the Relational DataBases tutorial to learn PostgreSQL by building a Mario Cart Database

## For instructions on how to install PostgreSql on your linux machine:
https://cloudinfrastructureservices.co.uk/how-to-install-postgresql-on-ubuntu-22-04-server/

## Once succesfully installed, you need to log in to PostgreSQL
using the default postgres user
```
$ sudo su - postgres
```
## list available databases
```
\l
```
there are three by default; postgres, template0, and template1
## create your own database
```
CREATE DATABASE  database_name;
```
The capitalized words are keywords telling PostgreSQL what to do.
The name of the database is the lowercase word.
Note that all commands need a semi-colon at the end.
## You need to connect to a database to add information
```
\c database_name
```
## A DB is made up of tables that hold data. List tables with display property:
```
\d
```
## Create a new table
```
CREATE TABLE table_name();
```
## View more information about a table
```
\d table_name
```
## Add columns
```
ALTER TABLE table_name ADD COLUMN column_name DATATYPE;
```
## Remove columns
```
ALTER TABLE table_name DROP COLUMN column_name;
```
## Rename columns
```
ALTER TABLE table_name RENAME COLUMN column_name TO new_name;
```
## Insert rows into columns;row contain the actual data
```
INSERT INTO table_name(column_1, column_2) VALUES(value1, value2);
```
## View data in a table(rows) by querryng it using Select method; * to view all columns;
```
SELECT  * table_name;
```
