# Notes
## Github Assignment
The cycle of pulling, editing, committing, and pushing using git.
1. verify you have the latest code (git pull)
1. Refactor, test, and/or implement a small portion of cohesive code (test code test)
1. Commit and push (git commit git push)
1. Repeat

git pull: gets the most recent version (from GitHub)

git commit: commits the changes made. You get to add a message to it
git commit -am "your comment goes here"

git push: pushes the changes to GitHub


## AWS Assignment
*Command to remote into server: ssh -i [path-file] ubuntu@[ip-address]
*Server IP: http://52.207.215.80/


## HTML Structure Assignment
Look in the code to see how to make each one
<h1>Landon Whitaker</h1> 
^^ creates a header
<div><a href="BYU.edu">BYU</a></div> 
^^ creates a hyperlink
  <ul>
        <li>apples</li> 
        <li>bananas</li>
        <li>oranges</li>
      </ul>   
^^ ul is an unordered list, li gets the elements of the list /ul ends the list
<p><img src="https://img.buzzfeed.com/buzzfeed-static/complex/images/Y19jcm9wLGhfMTY4MSx3XzI5ODgseF8xMSx5Xzcy/ccxzyc8kzae1lhun8imc/justin-jefferson-griddy-dance.jpg?downsize=1840:*&output-format=auto&output-quality=auto" width = "300" height = "200"></p> 
^^ creates an image of a man griddying

## HTML Input Assignment
| Element    | Meaning                          | Example                                        |
| ---------- | -------------------------------- | ---------------------------------------------- |
| `form`     | Input container and submission   | `<form action="form.html" method="post">`      |
| `fieldset` | Labeled input grouping           | `<fieldset> ... </fieldset>`                   |
| `input`    | Multiple types of user input     | `<input type="" />`                            |
| `select`   | Selection dropdown               | `<select><option>1</option></select>`          |
| `optgroup` | Grouped selection dropdown       | `<optgroup><option>1</option></optgroup>`      |
| `option`   | Selection option                 | `<option selected>option2</option>`            |
| `textarea` | Multiline text input             | `<textarea></textarea>`                        |
| `label`    | Individual input label           | `<label for="range">Range: </label>`           |
| `output`   | Output of input                  | `<output for="range">0</output>`               |
| `meter`    | Display value with a known range | `<meter min="0" max="100" value="50"></meter>` |


## Midterm Review
- 3 ways to put Javascript on HTML:
'''
<div onclick = '1+1' />
'''
''' 
<script>1+1</script>
'''
<script src = 'main.js'/>
 
- Java (Arrow function syntax)
- CSS box model (PBM)
- CSS flex !!
- Console commands
- Promise & filter & match Javascript : / indicates start of a regex
- textContent HTML
- = is not proper notation for objects. You need to use a colon :
- JSON
- DNS records/record types - A record maps into IP address from a hostname
- TXT stores a text string not used a lot - SOA link DNS records to someone else- CNAME is a hostname. Links an alias to a hostname cow.com -> dog.com
- Javascript function syntax
- CSS: .someClass selects the class that is declared in HTML


## JavaScript Array Objects

JavaScript array objects represent sequences of other objects and primitives.
Members of an array can be referenced using a zero-based index.
Arrays can be created using the Array constructor or array literal notation.
Example:

javascript
const a = [1, 2, 3];
console.log(a[1]); // OUTPUT: 2
console.log(a.length); // OUTPUT: 3
Object Functions

Array objects have various static functions for manipulation.
Some notable functions include push, pop, slice, sort, values, find, forEach, reduce, map, filter, every, and some.
Function Definitions:

javascript
Copy code
function push(item) {
  // Add an item to the end of the array
}

function pop() {
  // Remove an item from the end of the array
}

function slice(start, end) {
  // Return a sub-array
}

function sort(compareFunction) {
  // Run a function to sort an array in place
}

function values() {
  // Creates an iterator for use with a for of loop
}

function find(callback) {
  // Find the first item satisfied by a test function
}

function forEach(callback) {
  // Run a function on each array item
}

function reduce(callback, initialValue) {
  // Run a function to reduce each array item to a single item
}

function map(callback) {
  // Run a function to map an array to a new array
}

function filter(callback) {
  // Run a function to remove items
}

function every(callback) {
  // Run a function to test if all items match
}

function some(callback) {
  // Run a function to test if any items match
}

## JSON
A JSON document contains one of the following data types:

Type	    Example
string	  "crockford"
number	  42
boolean 	true
array	    [null,42,"crockford"]
object	  {"a":1,"b":"crockford"}
null	    null

Example JSON document:
{
  "class": {
    "title": "web programming",
    "description": "Amazing"
  },
  "enrollment": ["Marco", "Jana", "فَاطِمَة"],
  "start": "2025-02-01",
  "end": null
}

You can convert JSON to, and from, JavaScript using the JSON.parse and JSON.stringify functions.

const obj = { a: 2, b: 'crockford', c: undefined };
const json = JSON.stringify(obj);
const objFromJson = JSON.parse(json);

console.log(obj, json, objFromJson);

// OUTPUT:
// {a: 2, b: 'crockford', c: undefined}
// {"a":2, "b":"crockford"}
// {a: 2, b: 'crockford'}

## JS Console
If you are trying to see how long a piece of code is running you can wrap it with time and timeEnd calls and it will output the duration between the time and timeEnd calls:

console.time('demo time');
// ... some code that takes a long time.
console.timeEnd('demo time');
// OUTPUT: demo time: 9762.74 ms

To see how many times a block of code is called you can use the count function:

console.count('a');
// OUTPUT: a: 1
console.count('a');
// OUTPUT: a: 2
console.count('b');
// OUTPUT: b: 1

## JS with HTML
Add Javascript to HTML by using it within a script:
```
<head>
  <script src="javascript.js"></script>
</head>
<body>
  <button onclick="sayHello()">Say Hello</button>
  <button onclick="sayGoodbye()">Say Goodbye</button>
  <script>
    function sayGoodbye() {
      alert('Goodbye');
    }
  </script>
</body>
```
## variables and such

Variables are declared using either the let or const keyword. let allows you to change the value of the variable while const will cause an error if you attempt to change it. var is old and not used anymore

Type	    Meaning
Null	    The type of a variable that has not been assigned a value.
Undefined	The type of a variable that has not been defined.
Boolean 	true or false.
Number	  A 64-bit signed number.
BigInt	  A number of arbitrary magnitude.
String	  A textual sequence of characters.
Symbol	  A unique value.
Type	Use	Example
Object	A collection of properties represented by name-value pairs. Values can be of any type.	{a:3, b:'fish'}
Function	An object that has the ability to be called.	function a() {}
Date	Calendar dates and times.	new Date('1995-12-17')
Array	An ordered sequence of any type.	[3, 'fish']
Map	A collection of key-value pairs that support efficient lookups.	new Map()
JSON	A lightweight data-interchange format used to share information across programs.	{"a":3, "b":"fish"}


| Type      | Use                                                     | Example                   |
|-----------|---------------------------------------------------------|---------------------------|
| Object    | A collection of properties represented by name-value pairs. Values can be of any type. | `{a:3, b:'fish'}`        |
| Function  | An object that has the ability to be called.            | `function a() {}`        |
| Date      | Calendar dates and times.                                | `new Date('1995-12-17')` |
| Array     | An ordered sequence of any type.                         | `[3, 'fish']`             |
| Map       | A collection of key-value pairs that support efficient lookups. | `new Map()`          |
| JSON      | A lightweight data-interchange format used to share information across programs. | `{"a":3, "b":"fish"}`   |

| Function       | Meaning                                                                       |
|----------------|-------------------------------------------------------------------------------|
| length         | The number of characters in the string.                                       |
| indexOf()      | Returns the starting index of a given substring within the string.            |
| split()        | Splits the string into an array on the given delimiter string.                |
| startsWith()   | Returns true if the string starts with a given prefix.                         |
| endsWith()     | Returns true if the string ends with a given suffix.                           |
| toLowerCase()  | Converts all characters in the string to lowercase.

ex:

const s = 'Example:조선글';

console.log(s.length);
// OUTPUT: 11
console.log(s.indexOf('조선글'));
// OUTPUT: 8
console.log(s.split(':'));
// OUTPUT: ['Example', '조선글']
console.log(s.startsWith('Ex'));
// OUTPUT: true
console.log(s.endsWith('조선글'));
// OUTPUT: true
console.log(s.toLowerCase());
// OUTPUT: example:조선글

## Functions

Here are examples of assigning functions to variables, as well as using functions as parameters and return values.

// Anonymous declaration of the function that is later assigned to a variable
const add = function (a, b) {
  return a + b;
};

// Function that logs as a side effect of its execution
function labeler(label, value) {
  console.log(label + '=' + value);
}

// Function that takes a function as a parameter and then executes the function as a side effect
function addAndLabel(labeler, label, adder, a, b) {
  labeler(label, adder(a, b));
}

// Passing a function to a function
addAndLabel(labeler, 'a+b', add, 1, 3);
// OUTPUT: a+b=4

// Function that returns a function
function labelMaker(label) {
  return function (value) {
    console.log(label + '=' + value);
  };
}

// Assign a function from the return value of the function
const nameLabeler = labelMaker('name');

// Calling the returned function
nameLabeler('value');
// OUTPUT: name=value

## Arrow function
The following two invocations of sort are equivalent.

const a = [1, 2, 3, 4];

// standard function syntax
a.sort(function (v1, v2) {
  return v1 - v2;
});

// arrow function syntax
a.sort((v1, v2) => v1 - v2);



debounce function.

The point of a debounce function is to only execute a specified function once within a given time window. Any requests to execute the debounce function more frequently than this will case the time window to reset. This is important in cases where a user can trigger expensive events thousands of times per second. Without a debounce the performance of your application can greatly suffer.

## Objects / classes

A JavaScript object represents a collection of name value pairs referred to as properties. The property name must be of type String or Symbol, but the value can be of any type. Objects also have common object-oriented functionality such as constructors, a `this` pointer, static properties and functions, and inheritance.

Objects can be created with the new operator. This causes the object's constructor to be called. Once declared you can add properties to the object by simply referencing the property name in an assignment. Any type of variable can be assigned to a property. This includes a sub-object, array, or function. The properties of an object can be referenced either with dot (`obj.prop`) or bracket notation (`obj['prop']`).

```js
const obj = new Object({ a: 3 });
obj['b'] = 'fish';
obj.c = [1, 2, 3];
obj.hello = function () {
  console.log('hello');
};

console.log(obj);
// OUTPUT: {a: 3, b: 'fish', c: [1,2,3], hello: func}
```

The ability to dynamically modify an object is incredibly useful when manipulating data with an indeterminate structure.

⚠ Note the different uses of the term `object`. Object can refer to the standard JavaScript objects (e.g. `Promise, Map, Object, Function, Date, ...`), or it can refer specifically to the JavaScript Object object (i.e. `new Object()`), or it can refer to any JavaScript object you create (e.g. `{a:'a', b:2}` ). This overloaded usage can be a bit confusing.

### Object-literals

You can also declare a variable of object type with the `object-literal` syntax. This syntax allows you to provide the initial composition of the object.

```js
const obj = {
  a: 3,
  b: 'fish',
};
```

### Object functions

Object has several interesting static functions associated with it. Here are some of the commonly used ones.

| Function | Meaning                             |
| -------- | ----------------------------------- |
| entries  | Returns an array of key value pairs |
| keys     | Returns an array of keys            |
| values   | Returns an array of values          |

```js
const obj = {
  a: 3,
  b: 'fish',
};

console.log(Object.entries(obj));
// OUTPUT: [['a', 3], ['b', 'fish']]
console.log(Object.keys(obj));
// OUTPUT: ['a', 'b']
console.log(Object.values(obj));
// OUTPUT: [3, 'fish']
```

### Constructor

Any function that returns an object is considered a `constructor` and can be invoked with the `new` operator.

```js
function Person(name) {
  return {
    name: name,
  };
}

const p = new Person('Eich');
console.log(p);
// OUTPUT: {name: 'Eich'}
```

Because objects can have any type of property value you can create methods on the object as part of its encapsulation.

```js
function Person(name) {
  return {
    name: name,
    log: function () {
      console.log('My name is ' + this.name);
    },
  };
}

const p = new Person('Eich');
p.log();
// OUTPUT: My name is Eich
```

### This pointer

Notice in the last example the use of the keyword `this` when we referred to the name property (`this.name`). The meaning of `this` depends upon the scope of where it is used, but in the context of an object it refers to a pointer to the object. We will talk more about the `this` pointer in the instruction on scope.

### Classes

You can use classes to define objects. Using a class clarifies the intent to create a reusable component rather than a one-off object. Class declarations look similar to declaring an object, but classes have an explicit constructor and assumed function declarations. The person object from above would look like the following when converted to a class.

```js
class Person {
  constructor(name) {
    this.name = name;
  }

  log() {
    console.log('My name is ' + this.name);
  }
}

const p = new Person('Eich');
p.log();
// OUTPUT: My name is Eich
```

You can make properties and functions of classes private by prefixing them with a `#`.

```js
class Person {
  #name;

  constructor(name) {
    this.#name = name;
  }
}

const p = new Person('Eich');
p.#name = 'Lie';
// OUTPUT: Uncaught SyntaxError: Private field '#name' must be declared in an enclosing class
```

### Inheritance

Classes can be extended by using the `extends` keyword to define inheritance. Parameters that need to be passed to the parent class are delivered using the `super` function. Any functions defined on the child that have the same name as the parent override the parent's implementation. A parent's function can be explicitly accessed using the `super` keyword.

```js
class Person {
  constructor(name) {
    this.name = name;
  }

  print() {
    return 'My name is ' + this.name;
  }
}

class Employee extends Person {
  constructor(name, position) {
    super(name);
    this.position = position;
  }

  print() {
    return super.print() + '. I am a ' + this.position;
  }
}

const e = new Employee('Eich', 'programmer');
console.log(e.print());
// OUTPUT: My name is Eich. I am a programmer