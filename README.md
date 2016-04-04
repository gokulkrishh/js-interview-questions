# Javascript Interview Questions

*Repo contains basic & famous interview questions in javascript*


### Table of Contents
1. [Global & Local Variables](#global-and-local-variables)
1. [Hoisting](#hoisting)
1. [Operators](#operators)    
1. [Closures](#closures)    
1. [Arrays](#arrays)
1. [Objects](#objects)
1. [Prototype](#prototype)


## Global and Local Variables

- What is the output of the below program and why ?

```javascript

var foo = 10;

function myFunz() {
  foo = 11;
  console.log(foo); //print
}

console.log(foo); //print

myFunz();

console.log(foo); //print

```

## Hoisting

- What is the output of the below program and why ?

```javascript

myFunz(); //Will this function execute if yes, what is the output or if no why ?

function myFunz() {
  console.log(bar); //print
  var bar = 11;
  console.log(bar); //print
}

```

## Operators

- What will be output of below program and why ?

```javascript

console.log(0 == 1);

console.log(0 == "0");

console.log(0 === "0");

console.log(true == 1);

console.log(false == 0);

console.log(1 + 2 + "3");

console.log(1 + "2" + "3");

console.log("1" + 2);

console.log("1" + "3" + 2);

```

**[⬆ back to top](#table-of-contents)**


## Closures

- What is the output of the below program and why ?

```javascript

function parent(foo, bar) {
  var x = foo;

  function child() {
    console.log(x); //print
    console.log(foo); //print
    console.log(bar); //print
  }

  console.log(x); //print

  child();
}

parent();

```

- Fix the below program to print values from 0 to 9

```javascript

for (var i = 0; i < 9; i++) {
  setTimeout(function () {
    console.log(); //Should print from 0 to 9
  }, 0);
}

```

**[⬆ back to top](#table-of-contents)**


## Arrays

- How will you tell below input in the function is array or not ?

```javascript

function myFunz(x, y) {
  //write a method to find given input is array or not
  //If not array, print x & y type as well
}

var arr = [1, 2, 3];

var obj = {
  name: "gokul",
  age: 24
};

myFunz(arr, obj);

```

**[⬆ back to top](#table-of-contents)**


- Find ```max``` and ```min``` value in an array ?

- Write a program to remove duplicate value in an array

- Write a program to search an element in an array and optimize it to the most efficient solution and explain its complexity  

## Objects

- Write a function to do deep copy of the given object

- Write a function to compare two objects


## Prototype

- Write a class in javascript and its properties and methods should be inheritable by other functions

- How will you extend a method in javascript ?


**[⬆ back to top](#table-of-contents)**


### Contributions

If you find an issue, please file it. PR's are most welcome ;)
