How to Install Postgres in Docker

1. docker pull postgres
2. docker run --name learn_postgres -e POSTGRES_PASSWORD=mysecretpassword -p 5433:5432 -d postgres
3. docker exec -it learn_postgres bash
   su - postgres
   psql

Commands :-

\l - list all existing databases
CREATE DATABASE <DB NAME>; - to create new Database
\c <DB NAME>; - to Change Databse
DROP DATABASE <DB NAME>; - to Delete Database
CREATE TABLE <TABLE NAME> (id INT,name VARCHAR(200),city VARCHAR(100)) - to create table
\d <TABLE NAME> - to show table data
INSERT INTO <TABLE NAME> (id,name,city) VALUES (1,'Iphone','Ahmedabad'); - to insert data into table
SELECT \* FROM <TABLE NAME> - to show all data from table
SELECT <COLUMN NAME,COLUMN NAME> from <TABLE NAME>; - to show perticuler column of table
UPDATE <TABLE NAME> SET city = 'USA' WHERE id=2; - to update data
DELETE FROM <TABLE NAME> WHERE name='raju'; - to delete perticuler data from table
ALTER TABLE <TABLE NAME> ADD COLUMN <COLUMN NAME DATATYPE> - add column
ALTER TABLE <TABLE NAME> DROP COLUMN <COLUMN NAME> - drop column
ALTER TABLE <TABLE NAME> RENAME COLUMN <COLUMN NAME> TO <NEW COLUMN NAME> - rename column name
RENAME TABLE <TABLE NAME> TO <NEW TABLE NAME> - rename table name
ALTER TABLE <TABLE NAME> ALTER COLUMN <COLUMN NAME> SET DATA TYPE <DATATYPE> - change data type
ALTER TABLE <TABLE NAME> ADD COLUMN <COLUMN NAME DATATYPE> CHECK LENGTH(COLUMN NAME) >= 10 - to check mo number must be 10 or greater

Constraints :-

PRIMARY KEY,NOT NULL,DEFAULT,SERIAL(AUTO INCREMENT),

Caluse :-

WHERE,OR,AND,IN,BETWEEN
DISTINCT - for unique Values
ORDER BY - for show data in ascending,descending
LIMIT - restrict data
LIKE - for show data exact

Aggregate Functions :-

COUNT,SUM,AVG,MIN,MAX

String Functions :-

CONCAT,CONCAT_WS,SUBSTR,LEFT,RIGHT,UPPER,LOWER,TRIM,POSITION,REPLACE,REVERSE,LENGTH
