## :dart: How to pass children in React :dart:

##### in app.js
![Image of props and state](https://github.com/miaypc/Notes/blob/master/images/app.png)
#### in another.js
![Image of props and state](https://github.com/miaypc/Notes/blob/master/images/example.png)


## :rainbow: Databases :rainbow:

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
![Image of props and state](https://github.com/miaypc/Notes/blob/master/images/onetoone.png)

one-to-many
![Image of props and state](https://github.com/miaypc/Notes/blob/master/images/onetomany.png)

many-to-many
![Image of props and state](https://github.com/miaypc/Notes/blob/master/images/nonton.png)
![Image of props and state](https://github.com/miaypc/Notes/blob/master/images/addonemore.png)


Example:
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

#### :bangbang: Keep in Mind That...
! Semicolon is the standard way to separate each SQL statement in database systems that allow more than one SQL statement to be executed in the same call to the server.

! SQL keywords are NOT case sensitive: select is the same as SELECT


## :shipit: Node.js  :shipit:

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

_This code tells the computer to write "Hello World!" if anyone (e.g. a web browser) tries to access your computer on port 3000_


### Express

is a web framework for Node.js


_to install express_

`npm install express --save`


You can also use *nodemon* to monitor your project source code and automatically restart your Node.js server whenever it changes.

`npm i -D nodemon`

Node express https://gist.github.com/lflachs/d0ab1e5002a37aef5177252125216fad#file-node-express-L8


### Basic routing

Routing refers to determining how an application responds to a client request to a particular endpoint, which is a URI (or path) and a specific HTTP request method (GET, POST, and so on).

Each route can have one or more handler functions, which are executed when the route is matched.

Route definition takes the following structure:

`app.METHOD(PATH, HANDLER)`


**Where:**

* app is an instance of express.
* METHOD is an HTTP request method, in lowercase.
* PATH is a path on the server.
* HANDLER is the function executed when the route is matched.


#### The following examples illustrate defining simple routes.

_Respond with Hello World! on the homepage:_

``` 
app.get('/', function (req, res) {
  res.send('Hello World!')
}) 
```

_Respond to POST request on the root route (/), the application’s home page:_

```
app.post('/', function (req, res) {
  res.send('Got a POST request')
})
```





