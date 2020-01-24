# 🧠 topoftheweek  🧠


This week we worked on our projects

## What is Git

Git is ~~GitHub~~ a system for tracking changes in a code. It was created by Linus Torvalds.
_____
### Some commands learned:

1. Create repositories
##### `git init`
Turn an existing directory into a git repository
##### `git clone [url]`
Clone (download) a repository that already exists on
GitHub.

2. Work with branches
#### `git branch branch-name`
create a new branch
#### `git checkout branch-name`
switch to another branch
####  `git branch -d branch-name`
delete the specified branch

3. Pull and push

First of all we pull all the changes from the master by going to the master branch `git checkout master`. Then we execute `git pull` to update our current local working branch with all new commits from the corresponding remote branch on GitHub. 
Then we open code edditor `open .` and make changes to the code.
After all changes are done we check modified files in working directory`git status`.
Next steps are: 
* `git checkout -b branch-name`
create a new branch and switch to it
* `git add .`
* `git commit -m "what changes were done"`
* `git push origin branch-name`

! IMPORTANT 
**never push or delete master**

### Some essentials:
[Git cheatsheat](https://education.github.com/git-cheat-sheet-education.pdf)


___________
## Basic Java Script 
# Variables
#### 📦 Variables are containers for storing data values

### Declering variables : 
- unique name (identifiers)
- descriptive and short
- can contain letters, digits, underscores, and dollar signs.
- must begin with a letter
- or begin with $ and _ 
- case sensitive (y and Y are different variables)
- eserved words (like JavaScript keywords) cannot be used as names

### Data types :
- string
- number 
- boolean
- objects and more

### Declering variables 
### LET
this keyword signals that the variable can be re-assigned a different value (CAN be changed)
### CONST
CAN *NOT* be reassigned 
variables can be declared without a value

##### String concatanation with variables 
               let myName = "Melina";
               console.log("My name is "+ myName + " .");

##### String interpolation 
               const myName = "Linn";
               console.log( ` My name is ${myName} ` );


## ⭐ SCOPE ⭐
- defines where variable can be accessed or referenced

{...}block - cod found inside a set of curly brackets. Blocks help to group 1 or more statements together. 
### ⭐ 1. Global scope (global variables)
variables declared *outside* of the block. (can be accesed by any code in the program)

### ⭐ 2. Block scope (local variables)
variable defined *inside* of the block, it's only accesable from inside the block () withing curly brackets.(good practice)



### ✨✨Scope polution ✨✨
too many global variables in the global scope. Messy code



## Manipulating the DOM 
#### (Document Object Model) -the data representation of the objects that comprise the structure and content of a document on the web

### Selecting elements from HTML 

### 1. by ID
let element = document.getElementById("id")

### 2. by tag name
let elements = document.getElement*s*ByTagName("name")

### 3. by class 
let elements = document.getElement*s*ByClassName("name")

### Most useful  : 
 ❗   documents.querySelectorAll(".class")
return all elements withing that class (a collection, need to use loop to go through every element)

 ❗  documents.querySelectorAll("#tag")

### To manipulate html content 
ex:
- .innerHTML() - adding html tags
- .textContent() 
- .createElement()
- .removeChild()
- .appendChild()





## Arrays 
📦 = [🥝, 🍌, 🥚, 🍩];

Used to store multiple values in a single variable, in square brackets, can be storred in a variable.

0️⃣❗Arrays are zero-indexed: the first element of an array is at index 0 , and the last element is at the index equal to the value of the array's length property minus 1

Any type of data can be included in an Array :

          let myArray = ["example", 3, true, "another example but longer", 666 ]

### Accessing elements : 
      
               let myArray = ["example", 3, true, "another example but longer", 666 ]
               myArray[2] = true,
               myArray[4] = "666",
               (If you try to acces element on index 5 it will be undefined.)

### Accessing individual character :
          let hello = "welcome"
          console.log( hello[6] ) // output = e

### Update element : 

          let groceries = ["banana", "egg", "milk"];
          groceries[1] = "avocados";
          console.log(groceries)  // output = ["banana", "avocados", "milk"]
     
Most popular array methods (actions that can be used on arrays)
- .length
- .push()
- .pop()
- .shift()
- .unshift()
- .slice()
- .indexOf()
- .splice()

### List of popular methods :
https://www.w3schools.com/js/js_array_methods.asp

### Nested arrays - arrays containing other arrays 
ex:

              const myArray = [
                [1,2],
                [3,4],
                [5,6]
                [true, false],
                ["yes","no"]
            ];
            console.log(myArray[3,1])  // output true
            
            
            

more info : https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array            






## Objects 
🚗: 
{🔑:100€,
🔑:red,
🔑🏎️: no};

#### store various keyed collections, almost everything can be an object, regular expressions, arrays, functions, objects are also objects :) 


Objects have *properties* (it can be a string, number, boolen etc ) and *methods* (actions that can be used on objects).

### syntax 
       let/const objectname = { 
              key : property ,
        };

Example :

          let avocado = {
                color inside : "white" ,
                color outside : "brown" ,
                origin: "New Zeland" ,
                taste: "omg"
           };

               let kiwi = {
                 color inside : "green" ,
                 color outside : "brown",
                 origin: "New Zeland",
                 taste: "yummy"
               };

#### Object methods include 
- Object.keys(), 
- Object.values(), 
- Object.create, 
- Object.assign() 
etc.

#### More on the topic : 
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object


### ⭕ Looping through objects (FOR ... IN LOOP) ⭕
example : 

                const student = {
                   name : "Yannic",
                   age : 25,
                   nationality : "swedish",
                   class2020 : true
                 };
 
                     for (const propName in student){
                            console.log(propName);
                      };
 
 more info: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/for...in
 
 
 
 
 Useful links  👋👋
 1. https://developer.mozilla.org/en-US/
 2. https://www.w3schools.com/
 3. https://caniuse.com/#
 4. https://htmlcheatsheet.com/js/
 5. https://www.youtube.com/watch?v=hdI2bqOjy3c&list=PLillGF-RfqbbnEGy3ROiLWk7JMCuSyQtX - very nicely made JS video courses from the very start :) 
 6. https://www.youtube.com/watch?v=gPDk7_l_7WE - watch this is you're feeling bad about your code/skills/life 🤯🤬🥺
 
 
 
 
 
 
 
 
 
 
 


____
## Loop:

1. **while** 

```
while (condition) {
  
  
  // code
  
  
}
```

2. **do while**


*this code will execute at least once, even if the condition is false*

```
do {

  // loop body
  
} while (condition);
```


3. **for (begin; condition; step)** 

```
for (let i = 0; i < 3; i++){

  alert(i);
  
}
```

## A "switch" statement

The switch statement can replace multiple **if** checks.

**Syntax**

```
switch(x) {

  case 'value1':  // *if (x === 'value1')*
  
    
    break

  case 'value2':  // *else if (x === 'value2')*
 
    break

  default:     // *else* 

    break
    
}
```

## Functions

Quite often we need to perform a similar action in many places of the script.
Functions can 

* A **function declaration** looks like this:

```
function sum(a, b) {
  return a + b;
}
```

* Another syntax for creating a function that is called a **Function Expression**.

```
let sayHi = function() {
  alert( "Hello" );
};
```

* There’s another syntax for creating functions, arrow functions.

### !IMPORTANT
A Function Expression is created when the execution reaches it and is usable only from that moment.
A Function Declaration can be called earlier than it is defined.


For example, this works:
```
sayHi("John"); // Hello, John

function sayHi(name) {
  alert( `Hello, ${name}` );
}
```



