## How to pass children in React

##### in app.js
![Image of props and state](https://github.com/miaypc/Notes/blob/master/images/app.png)
#### in another.js
![Image of props and state](https://github.com/miaypc/Notes/blob/master/images/example.png)


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

Useful links: (https://www.notion.so/Databases-e03650e7b504439891cd80b51f9e4a91)


## What is a DB model?
#### A database model describes how data can be stored, organized and accessed in a database.

## What is a Relational DB model?
#### A Relational db Model is the type of database model that describes Relational Databases.
#### It describes all the tables, relations between the tables and data constraints.

There are 3 types of relations:

one-to-one

one-to-many

many-to-many

![Image of props and state](https://github.com/miaypc/Notes/blob/master/images/database.png)



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


## Node.js 

Node.js is an open source server environment.

Node.js allows you to run JavaScript on the server.

### Node.js Modules

Consider modules to be the same as JavaScript libraries.

A set of functions you want to include in your application.

To include a module, use the **require()** function with the name of the module:

`const http = require('http');`

Now your application has access to the HTTP module, and is able to create a server.

`const http = require('http');`

`http.createServer(function (req, res) {`

 ` res.writeHead(200, {'Content-Type': 'text/html'});`
 
 ` res.end('Hello World!');`
 
`}).listen(3000);`

This code tells the computer to write "Hello World!" if anyone (e.g. a web browser) tries to access your computer on port 3000



