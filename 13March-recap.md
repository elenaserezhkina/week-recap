## Databases

### A database is an **organized** collection of **data**.


The database is composed of tables

Each table is represented by a schema

**Example**
 
 User
`{
id INT PRIMARY_KEY
lastname VARCHAR
firstname VARCHAR
age INT
}`


| id            | last name     | age   |
| ------------- |:-------------:| -----:|
| 1             | Pin           |  25   |
| 2             | Smith         |  30   |


Each table contains **fields/columns**
Each line is called a **tuple**
Each tuple has (usually) a unique identifier, called a **primary key**


## Database Management Systems

There are two main types: **Relational and Non Relational (NoSQL) databases.**


| id            | last name     | age   |
| ------------- |:-------------:| -----:|
| 1             | Pin           |  25   |
| 2             | Smith         |  30   |


`knight : {
  $arthur : {
	  name: Arthur Pendragon,
	  age : 40,
    kingdom : {
      name : Logre,
      capital : Camelot,
      inhabitants : 100000 
    }
  }
}`





## :zap: Structure Query Language(SQL) :zap:
#### is a database query language used for storing and managing data in Relational DBMS

___________________

To run mysql:
`mysql -u root -p`

Create a database:
`mysql > CREATE DATABASE wild;`

List all DBs:
`SHOW DATABASES;`

List all tables in the currently selected database:
`SHOW TABLES;`


### :panda_face: Some of The Most Important SQL Commands
* SELECT - extracts data from a database
* UPDATE - updates data in a database
* DELETE - deletes data from a database
* INSERT INTO - inserts new data into a database
* CREATE DATABASE - creates a new database
* ALTER DATABASE - modifies a database
* CREATE TABLE - creates a new table
* ALTER TABLE - modifies a table
* DROP TABLE - deletes a table

#### Keep in Mind That...
! Semicolon is the standard way to separate each SQL statement in database systems that allow more than one SQL statement to be executed in the same call to the server.

! SQL keywords are NOT case sensitive: select is the same as SELECT








