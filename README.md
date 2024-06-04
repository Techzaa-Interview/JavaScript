# JavaScript Interview Questions and Answers <img src="https://upload.wikimedia.org/wikipedia/commons/9/99/Unofficial_JavaScript_logo_2.svg" alt="JavaScript Logo" width="50"/>

Welcome to the JavaScript Interview Questions repository! This collection of questions is designed to help you prepare for JavaScript-related interviews. The questions cover a wide range of topics, from basic to advanced, and include examples to illustrate the concepts. Whether you're a beginner or an experienced developer, this guide will help you brush up on your JavaScript skills and ace your next interview!

## Table of Contents

1. [🚀 Introduction](#introduction)
2. [🌟 Basic Questions](#basic-questions)
3. [🔢 Data Types](#data-types)
4. [⚙️ Functions](#functions)
5. [📚 Arrays](#arrays)
6. [🔵 Objects](#objects)
7. [🔧 Classes](#classes)
8. [🔍 Scope and Closures](#scope-and-closures)
9. [🖥️ DOM Manipulation](#dom-manipulation)
10. [⏳ Asynchronous Programming](#asynchronous-programming)
11. [❌ Error Handling](#error-handling)
12. [✨ ES6 Features](#es6-features)
13. [🎲 Miscellaneous](#miscellaneous)

## Introduction

JavaScript is a powerful programming language that is widely used for web development. It is a versatile language that can be used for both front-end and back-end development. JavaScript is known for its flexibility and dynamic nature, making it an essential skill for any developer.


### 🚀 Introduction - Basic Questions

1. **What is JavaScript?**
   - **Answer:** JavaScript is a versatile, high-level programming language primarily used for creating interactive elements on websites. It is an interpreted language, meaning it is executed line-by-line in the browser.

   - **Example:**
     ```html
     <script>
       alert("Hello, World!");
     </script>
     ```

2. **What are the main features of JavaScript?**
   - **Answer:** JavaScript features include:
     - Lightweight and interpreted
     - Dynamic typing
     - First-class functions
     - Prototype-based object orientation
     - Event-driven and asynchronous programming

   - **Example:**
     ```javascript
     const message = "Hello, World!";
     console.log(message); // Output: Hello, World!
     ```

3. **How do you include JavaScript in an HTML file?**
   - **Answer:** JavaScript can be included in an HTML file using the `<script>` tag. This tag can be placed in the `<head>` or `<body>` section of the HTML document.

   - **Example:**
     ```html
     <html>
     <head>
       <script>
         console.log("This is JavaScript in the head section");
       </script>
     </head>
     <body>
       <script>
         console.log("This is JavaScript in the body section");
       </script>
     </body>
     </html>
     ```

4. **What is the `console.log` method used for?**
   - **Answer:** The `console.log` method is used to print messages to the browser's console. It is commonly used for debugging purposes.

   - **Example:**
     ```javascript
     console.log("Hello, World!"); // Output: Hello, World!
     ```

5. **What is a variable in JavaScript, and how do you declare it?**
   - **Answer:** A variable in JavaScript is a container for storing data values. Variables are declared using the `var`, `let`, or `const` keywords.

   - **Example:**
     ```javascript
     var name = "Alice";
     let age = 25;
     const city = "New York";
     ```


6. **How do you write a comment in JavaScript?**
   - **Answer:** Comments in JavaScript can be single-line or multi-line. Single-line comments start with `//`, and multi-line comments are enclosed within `/*` and `*/`.

   - **Example:**
     ```javascript
     // This is a single-line comment
     /*
       This is a
       multi-line comment
     */
     ```


## Data Types
1. How can you check if a variable is an array in JavaScript?
   - **Answer:** You can check if a variable is an array using the `Array.isArray()` method.
   - **Example:**
     ```javascript
     let arr = [1, 2, 3];
     console.log(Array.isArray(arr)); // Output: true
     ```

2. What is the difference between `null` and `undefined`?
   - **Answer:** `null` is an explicitly assigned value that represents the absence of a value, while `undefined` means that a variable has been declared but has not been assigned a value.

3. How do you convert a string to a number in JavaScript?
   - **Answer:** You can convert a string to a number using the `parseInt()` or `parseFloat()` functions.
   - **Example:**
     ```javascript
     let str = '10';
     let num = parseInt(str);
     console.log(num); // Output: 10
     ```

4. What is the difference between `==` and `===` in JavaScript?
   - **Answer:** The `==` operator performs type coercion before comparing two values, while the `===` operator compares the values without type coercion.

5. What are the different ways to create an object in JavaScript?
   - **Answer:** Objects in JavaScript can be created using object literals, the `Object` constructor, or with a constructor function.
   - **Example:**
     ```javascript
     // Using object literal
     let obj1 = { key: 'value' };

     // Using Object constructor
     let obj2 = new Object();

     // Using constructor function
     function Person(name) {
       this.name = name;
     }
     let obj3 = new Person('John');
     ```

6. What is the difference between `let` and `var`?
   - **Answer:** `let` is block-scoped, while `var` is function-scoped. Variables declared with `let` are not hoisted to the top of the block.

7. What is a closure in JavaScript?
   - **Answer:** A closure is a function that has access to its own scope, the outer function's scope, and the global scope.

8. How can you create a copy of an object in JavaScript?
   - **Answer:** You can create a copy of an object using the `Object.assign()` method or the spread operator (`...`).
   - **Example:**
     ```javascript
     let obj1 = { key: 'value' };
     let obj2 = Object.assign({}, obj1);
     // or
     let obj3 = { ...obj1 };
     ```

9. How do you check if a property exists in an object?
   - **Answer:** You can check if a property exists in an object using the `hasOwnProperty()` method or by directly accessing the property.
   - **Example:**
     ```javascript
     let obj = { key: 'value' };
     console.log(obj.hasOwnProperty('key')); // Output: true
     ```

10. What is the difference between `null` and `undefined`?
    - **Answer:** `null` is an explicitly assigned value that represents the absence of a value, while `undefined` means that a variable has been declared but has not been assigned a value.

## Functions
1. What is a higher-order function in JavaScript?
   - **Answer:** A higher-order function is a function that takes another function as an argument or returns a function as a result.

2. What is the difference between function declaration and function expression?
   - **Answer:** Function declarations are hoisted to the top of the script, while function expressions are not hoisted.

3. How do you pass arguments to a function in JavaScript?
   - **Answer:** You can pass arguments to a function by placing them within the parentheses when calling the function.
   - **Example:**
     ```javascript
     function add(a, b) {
       return a + b;
     }
     console.log(add(1, 2)); // Output: 3
     ```

4. What is the difference between `function` and `=>` in JavaScript?
   - **Answer:** The `function` keyword creates a traditional function with its own `this` context, while arrow functions (`=>`) inherit the `this` context from the surrounding code.

5. What is a callback function?
   - **Answer:** A callback function is a function that is passed as an argument to another function and is executed after some operation has been completed.

6. How do you return a value from a function in JavaScript?
   - **Answer:** You can return a value from a function using the `return` statement.
   - **Example:**
     ```javascript
     function add(a, b) {
       return a + b;
     }
     console.log(add(1, 2)); // Output: 3
     ```

7. What is a recursive function?
   - **Answer:** A recursive function is a function that calls itself until a base condition is met.

8. How do you create a named function expression in JavaScript?
   - **Answer:** You can create a named function expression by giving the function a name when defining it.
   - **Example:**
     ```javascript
     let factorial = function factorial(n) {
       if (n === 0) {
         return 1;
       }
       return n * factorial(n - 1);
     };
     ```

9. What is the difference between `call()` and `apply()` methods?
   - **Answer:** Both `call()` and `apply()` are methods that allow you to call a function with a specified `this` value and arguments. The difference is in how arguments are passed. `call()` accepts an argument list, while `apply()` accepts a single array of arguments.

10. How do you create a function that returns another function in JavaScript?
    - **Answer:** You can create a function that returns another function by defining a function inside another function and returning it.
    - **Example:**
      ```javascript
      function outerFunction() {
        function innerFunction() {
          console.log('Inner function');
        }
        return innerFunction;
      }

      let inner = outerFunction();
      inner(); // Output: Inner function
      ```

Let's continue with more interview questions focusing on different topics:

## Arrays
1. How do you iterate over an array in JavaScript?
   - **Answer:** You can iterate over an array using a `for` loop, `forEach()`, `map()`, `filter()`, or `reduce()` methods.
   - **Example:**
     ```javascript
     let arr = [1, 2, 3];
     for (let i = 0; i < arr.length; i++) {
       console.log(arr[i]);
     }
     // Using forEach()
     arr.forEach(function(element) {
       console.log(element);
     });
     ```

2. How do you add an element to the beginning and end of an array in JavaScript?
   - **Answer:** You can use the `unshift()` method to add an element to the beginning of an array and the `push()` method to add an element to the end of an array.
   - **Example:**
     ```javascript
     let arr = [2, 3];
     arr.unshift(1); // arr is now [1, 2, 3]
     arr.push(4); // arr is now [1, 2, 3, 4]
     ```

3. How do you remove an element from the beginning and end of an array in JavaScript?
   - **Answer:** You can use the `shift()` method to remove an element from the beginning of an array and the `pop()` method to remove an element from the end of an array.
   - **Example:**
     ```javascript
     let arr = [1, 2, 3, 4];
     arr.shift(); // arr is now [2, 3, 4]
     arr.pop(); // arr is now [2, 3]
     ```

4. How do you find the index of an element in an array in JavaScript?
   - **Answer:** You can use the `indexOf()` method to find the index of an element in an array.
   - **Example:**
     ```javascript
     let arr = [1, 2, 3, 4];
     let index = arr.indexOf(3); // index is 2
     ```

5. How do you remove an element from a specific index in an array in JavaScript?
   - **Answer:** You can use the `splice()` method to remove elements from a specific index in an array.
   - **Example:**
     ```javascript
     let arr = [1, 2, 3, 4];
     arr.splice(1, 1); // remove 1 element at index 1
     // arr is now [1, 3, 4]
     ```

6. How do you check if an array includes a certain value in JavaScript?
   - **Answer:** You can use the `includes()` method to check if an array includes a certain value.
   - **Example:**
     ```javascript
     let arr = [1, 2, 3, 4];
     console.log(arr.includes(3)); // Output: true
     ```

7. How do you reverse an array in JavaScript?
   - **Answer:** You can use the `reverse()` method to reverse the elements of an array.
   - **Example:**
     ```javascript
     let arr = [1, 2, 3, 4];
     arr.reverse(); // arr is now [4, 3, 2, 1]
     ```

8. How do you flatten an array in JavaScript?
   - **Answer:** You can use the `flat()` method to flatten an array with nested arrays.
   - **Example:**
     ```javascript
     let arr = [1, [2, 3], 4, [5, 6]];
     let flattened = arr.flat(); // flattened is [1, 2, 3, 4, 5, 6]
     ```

9. How do you sort an array in JavaScript?
   - **Answer:** You can use the `sort()` method to sort an array.
   - **Example:**
     ```javascript
     let arr = [3, 1, 4, 1, 5, 9, 2, 6];
     arr.sort(); // arr is now [1, 1, 2, 3, 4, 5, 6, 9]
     ```

10. How do you check if all elements in an array satisfy a condition in JavaScript?
    - **Answer:** You can use the `every()` method to check if all elements in an array satisfy a condition.
    - **Example:**
      ```javascript
      let arr = [2, 4, 6, 8];
      let allEven = arr.every(function(element) {
        return element % 2 === 0;
      });
      console.log(allEven); // Output: true
      ```

## Objects
1. How do you access the properties of an object in JavaScript?
   - **Answer:** You can access the properties of an object using dot notation (`obj.property`) or bracket notation (`obj['property']`).
   - **Example:**
     ```javascript
     let obj = { key: 'value' };
     console.log(obj.key); // Output: value
     console.log(obj['key']); // Output: value
     ```

2. How do you add a new property to an object in JavaScript?
   - **Answer:** You can add a new property to an object by assigning a value to a new key.
   - **Example:**
     ```javascript
     let obj = { key1: 'value1' };
     obj.key2 = 'value2'; // obj is now { key1: 'value1', key2: 'value2' }
     ```

3. How do you remove a property from an object in JavaScript?
   - **Answer:** You can use the `delete` operator to remove a property from an object.
   - **Example:**
     ```javascript
     let obj = { key1: 'value1', key2: 'value2' };
     delete obj.key2; // obj is now { key1: 'value1' }
     ```

4. How do you iterate over the properties of an object in JavaScript?
   - **Answer:** You can iterate over the properties of an object using a `for...in` loop.
   - **Example:**
     ```javascript
     let obj = { a: 1, b: 2, c: 3 };
     for (let key in obj) {
       console.log(key + ': ' + obj[key]);
     }
     ```

5. How do you check if a property exists in an object in JavaScript?
   - **Answer:** You can use the `hasOwnProperty()` method to check if a property exists in an object.
   - **Example:**
     ```javascript
     let obj = { key: 'value' };
     console.log(obj.hasOwnProperty('key')); // Output: true
     ```

6. How do you create a copy of an object in JavaScript?
   - **Answer:** You can create a copy of an object using the `Object.assign()` method or the spread operator (`...`).

Certainly! Let's continue with more interview questions focusing on JavaScript:

## Classes
1. How do you create a class in JavaScript?
   - **Answer:** You can create a class using the `class` keyword.
   - **Example:**
     ```javascript
     class Person {
       constructor(name, age) {
         this.name = name;
         this.age = age;
       }

       greet() {
         console.log(`Hello, my name is ${this.name} and I am ${this.age} years old.`);
       }
     }

     let person = new Person('Alice', 30);
     person.greet(); // Output: Hello, my name is Alice and I am 30 years old.
     ```

2. How do you extend a class in JavaScript?
   - **Answer:** You can extend a class using the `extends` keyword.
   - **Example:**
     ```javascript
     class Student extends Person {
       constructor(name, age, grade) {
         super(name, age);
         this.grade = grade;
       }

       study() {
         console.log(`${this.name} is studying.`);
       }
     }

     let student = new Student('Bob', 20, 'A');
     student.greet(); // Output: Hello, my name is Bob and I am 20 years old.
     student.study(); // Output: Bob is studying.
     ```

3. What is the difference between a class and a constructor function in JavaScript?
   - **Answer:** Classes provide a more concise and clear syntax for creating objects and working with inheritance compared to constructor functions.

4. How do you create static methods in a class in JavaScript?
   - **Answer:** You can create static methods in a class by using the `static` keyword.
   - **Example:**
     ```javascript
     class MathUtils {
       static add(a, b) {
         return a + b;
       }
     }

     console.log(MathUtils.add(1, 2)); // Output: 3
     ```

5. How do you define getters and setters in a class in JavaScript?
   - **Answer:** You can define getters and setters using the `get` and `set` keywords.
   - **Example:**
     ```javascript
     class Circle {
       constructor(radius) {
         this.radius = radius;
       }

       get area() {
         return Math.PI * this.radius * this.radius;
       }

       set diameter(diameter) {
         this.radius = diameter / 2;
       }
     }

     let circle = new Circle(5);
     console.log(circle.area); // Output: 78.54
     circle.diameter = 10;
     console.log(circle.radius); // Output: 5
     ```

6. What is the difference between a static method and a prototype method in JavaScript classes?
   - **Answer:** Static methods are called on the class itself, while prototype methods are called on instances of the class.

7. How do you check if an object is an instance of a specific class in JavaScript?
   - **Answer:** You can use the `instanceof` operator to check if an object is an instance of a specific class.
   - **Example:**
     ```javascript
     let obj = new Person('Alice', 30);
     console.log(obj instanceof Person); // Output: true
     ```

8. How do you prevent a class from being instantiated in JavaScript?
   - **Answer:** You can prevent a class from being instantiated by making the constructor `private` or by throwing an error in the constructor.
   - **Example:**
     ```javascript
     class Singleton {
       constructor() {
         throw new Error('Use Singleton.getInstance() to get an instance.');
       }

       static getInstance() {
         if (!Singleton.instance) {
           Singleton.instance = new Singleton();
         }
         return Singleton.instance;
       }
     }

     let instance = Singleton.getInstance();
     ```

9. How do you create a private method in a class in JavaScript?
   - **Answer:** There is no direct way to create private methods in classes in JavaScript. However, you can use closures to achieve a similar effect.
   - **Example:**
     ```javascript
     class Counter {
       constructor() {
         let count = 0;
         this.increment = function() {
           count++;
           console.log(count);
         };
       }
     }

     let counter = new Counter();
     counter.increment(); // Output: 1
     ```

6. What is the purpose of the `super` keyword in JavaScript classes?
   - **Answer:** The `super` keyword is used to call the constructor or methods of a parent class.
   - **Example:**
     ```javascript
     class Animal {
       constructor(name) {
         this.name = name;
       }

       speak() {
         console.log(`${this.name} makes a noise.`);
       }
     }

     class Dog extends Animal {
       constructor(name, breed) {
         super(name);
         this.breed = breed;
       }

       speak() {
         super.speak();
         console.log(`${this.name} barks.`);
       }
     }

     let dog = new Dog('Rex', 'German Shepherd');
     dog.speak(); // Output: Rex makes a noise. Rex barks.
     ```

7. Can you explain the difference between `public`, `protected`, and `private` fields in JavaScript classes?
   - **Answer:** JavaScript currently supports public and private fields. Public fields are accessible from outside the class, while private fields (prefixed with `#`) are only accessible within the class.
   - **Example:**
     ```javascript
     class Car {
       #mileage = 0; // Private field

       constructor(brand) {
         this.brand = brand; // Public field
       }

       drive(distance) {
         this.#mileage += distance;
       }

       getMileage() {
         return this.#mileage;
       }
     }

     let myCar = new Car('Toyota');
     myCar.drive(100);
     console.log(myCar.getMileage()); // Output: 100
     console.log(myCar.#mileage); // SyntaxError: Private field '#mileage' must be declared in an enclosing class
     ```

## Scope and Closures
1. What is the difference between `var`, `let`, and `const` in terms of scope?
   - **Answer:** `var` is function-scoped, while `let` and `const` are block-scoped. `const` also indicates that the variable cannot be reassigned.
   - **Example:**
     ```javascript
     function example() {
       if (true) {
         var x = 10; // function-scoped
         let y = 20; // block-scoped
         const z = 30; // block-scoped
       }
       console.log(x); // Output: 10
       console.log(y); // ReferenceError: y is not defined
       console.log(z); // ReferenceError: z is not defined
     }
     example();
     ```

2. Can you explain the concept of closure in JavaScript?
   - **Answer:** A closure is a function that has access to its own scope, the scope of the outer function, and the global scope.
   - **Example:**
     ```javascript
     function outerFunction(outerVariable) {
       return function innerFunction(innerVariable) {
         console.log('Outer Variable:', outerVariable);
         console.log('Inner Variable:', innerVariable);
       };
     }

     const newFunction = outerFunction('outside');
     newFunction('inside'); // Output: Outer Variable: outside, Inner Variable: inside
     ```

3. How can closures be used to create private variables?
   - **Answer:** Closures can be used to create private variables by encapsulating the variables within a function scope.
   - **Example:**
     ```javascript
     function createCounter() {
       let count = 0; // Private variable

       return {
         increment: function() {
           count++;
           return count;
         },
         decrement: function() {
           count--;
           return count;
         },
         getCount: function() {
           return count;
         }
       };
     }

     const counter = createCounter();
     console.log(counter.increment()); // Output: 1
     console.log(counter.decrement()); // Output: 0
     console.log(counter.getCount()); // Output: 0
     console.log(counter.count); // Output: undefined
     ```

4. What is the temporal dead zone in JavaScript?
   - **Answer:** The temporal dead zone (TDZ) refers to the period between entering a scope and the point where a variable is declared. During this period, accessing the variable will result in a `ReferenceError`.
   - **Example:**
     ```javascript
     {
       // TDZ for `a`
       console.log(a); // ReferenceError: Cannot access 'a' before initialization
       let a = 3; // `a` is declared
     }
     ```

5. How do you create a module in JavaScript using closures?
   - **Answer:** You can create a module using an IIFE (Immediately Invoked Function Expression) that returns an object containing methods.
   - **Example:**
     ```javascript
     const module = (function() {
       let privateVar = 'I am private';

       function privateMethod() {
         console.log(privateVar);
       }

       return {
         publicMethod: function() {
           privateMethod();
         }
       };
     })();

     module.publicMethod(); // Output: I am private
     console.log(module.privateVar); // Output: undefined
     ```

## DOM Manipulation
1. How do you select an HTML element by its ID in JavaScript?
   - **Answer:** You can select an HTML element by its ID using the `document.getElementById()` method.
   - **Example:**
     ```javascript
     let element = document.getElementById('myElement');
     ```

2. How do you add a class to an HTML element in JavaScript?
   - **Answer:** You can add a class to an HTML element using the `classList.add()` method.
   - **Example:**
     ```javascript
     let element = document.getElementById('myElement');
     element.classList.add('newClass');
     ```

3. How do you create a new HTML element in JavaScript?
   - **Answer:** You can create a new HTML element using the `document.createElement()` method.
   - **Example:**
     ```javascript
     let newElement = document.createElement('div');
     newElement.textContent = 'Hello, World!';
     document.body.appendChild(newElement);
     ```

4. How do you remove an HTML element from the DOM in JavaScript?
   - **Answer:** You can remove an HTML element from the DOM using the `removeChild()` method.
   - **Example:**
     ```javascript
     let parentElement = document.getElementById('parent');
     let childElement = document.getElementById('child');
     parentElement.removeChild(childElement);
     ```

5. How do you add an event listener to an HTML element in JavaScript?
   - **Answer:** You can add an event listener to an HTML element using the `addEventListener()` method.
   - **Example:**
     ```javascript
     let button = document.getElementById('myButton');
     button.addEventListener('click', function() {
       alert('Button clicked!');
     });
     ```

6. How do you get the value of an input field in JavaScript?
   - **Answer:** You can get the value of an input field using the `value` property.
   - **Example:**
     ```javascript
     let input = document.getElementById('myInput');
     let value = input.value;
     console.log(value);
     ```

7. How do you set the value of an input field in JavaScript?
   - **Answer:** You can set the value of an input field using the `value` property.
   - **Example:**
     ```javascript
     let input = document.getElementById('myInput');
     input.value = 'New Value';
     ```

8. How do you change the content of an HTML element in JavaScript?
   - **Answer:** You can change the content of an HTML element using the `innerHTML` or `textContent` property.
   - **Example:**
     ```javascript
     let element = document.getElementById('myElement');
     element.innerHTML = '<p>New Content</p>';
     // or
     element.textContent = 'New Content';
     ```

9. How do you toggle a class on an HTML element in JavaScript?
   - **Answer:** You can toggle a class on an HTML element using the `classList.toggle()` method.
   - **Example:**
     ```javascript
     let element = document.getElementById('myElement');
     element.classList.toggle('active');
     ```

10. How do you prevent the default action of an event in JavaScript?
    - **Answer:** You can prevent the default action of an event using the `preventDefault()` method.
    - **Example:**
      ```javascript
      let link = document.getElementById('myLink');
      link.addEventListener('click', function(event) {
        event.preventDefault();
        console.log('Default action prevented.');
      });
      ```

## Asynchronous Programming
1. What is a promise in JavaScript?
   - **Answer:** A promise is an object representing the eventual completion or failure of an asynchronous operation.
   - **Example:**
     ```javascript
     let promise = new Promise(function(resolve, reject) {
       // Asynchronous operation
       if (success) {
         resolve(result);
       } else {
         reject(error);
       }
     });

     promise.then(function(result) {
       console.log(result);
     }).catch(function(error) {
       console.error(error);
     });
     ```

2. How do you create and use async/await in JavaScript?
   - **Answer:** You can create an async function using the `async` keyword and use `await` to wait for a promise to resolve.
  

 - **Example:**
     ```javascript
     async function fetchData() {
       try {
         let response = await fetch('https://api.example.com/data');
         let data = await response.json();
         console.log(data);
       } catch (error) {
         console.error(error);
       }
     }

     fetchData();
     ```

3. How do you handle multiple promises concurrently in JavaScript?
   - **Answer:** You can handle multiple promises concurrently using `Promise.all()`.
   - **Example:**
     ```javascript
     let promise1 = fetch('https://api.example.com/data1');
     let promise2 = fetch('https://api.example.com/data2');

     Promise.all([promise1, promise2])
       .then(function(results) {
         return Promise.all(results.map(result => result.json()));
       })
       .then(function(data) {
         console.log(data);
       })
       .catch(function(error) {
         console.error(error);
       });
     ```

4. What is the purpose of the `finally` method in promises?
   - **Answer:** The `finally` method is used to execute code regardless of the promise's outcome (resolved or rejected).
   - **Example:**
     ```javascript
     let promise = fetch('https://api.example.com/data');

     promise.then(function(response) {
       return response.json();
     }).catch(function(error) {
       console.error(error);
     }).finally(function() {
       console.log('Promise settled');
     });
     ```

5. How do you create a promise that resolves after a specified delay?
   - **Answer:** You can create a promise that resolves after a delay using `setTimeout`.
   - **Example:**
     ```javascript
     function delay(ms) {
       return new Promise(function(resolve) {
         setTimeout(resolve, ms);
       });
     }

     delay(2000).then(function() {
       console.log('Resolved after 2 seconds');
     });
     ```

6. What is the difference between `Promise.all` and `Promise.race`?
   - **Answer:** `Promise.all` waits for all promises to resolve or any to reject, while `Promise.race` resolves or rejects as soon as one promise resolves or rejects.
   - **Example:**
     ```javascript
     let promise1 = new Promise((resolve) => setTimeout(resolve, 100, 'first'));
     let promise2 = new Promise((resolve) => setTimeout(resolve, 200, 'second'));

     Promise.all([promise1, promise2]).then(console.log); // Output: ['first', 'second']
     Promise.race([promise1, promise2]).then(console.log); // Output: 'first'
     ```

7. How do you handle errors in asynchronous code using async/await?
   - **Answer:** You can handle errors in async functions using `try...catch`.
   - **Example:**
     ```javascript
     async function fetchData() {
       try {
         let response = await fetch('https://api.example.com/data');
         let data = await response.json();
         console.log(data);
       } catch (error) {
         console.error('Error:', error);
       }
     }

     fetchData();
     ```

8. How do you create a promise that rejects after a specified delay?
   - **Answer:** You can create a promise that rejects after a delay using `setTimeout`.
   - **Example:**
     ```javascript
     function delayReject(ms) {
       return new Promise(function(resolve, reject) {
         setTimeout(reject, ms, 'Rejected after delay');
       });
     }

     delayReject(2000).catch(function(reason) {
       console.error(reason);
     });
     ```

9. How do you use the `await` operator with non-promise values?
   - **Answer:** The `await` operator can be used with any value, and it will simply return that value if it is not a promise.
   - **Example:**
     ```javascript
     async function example() {
       let value = await 42;
       console.log(value); // Output: 42
     }

     example();
     ```

10. How do you handle promise rejection in JavaScript?
    - **Answer:** You can handle promise rejection using the `catch` method or by passing a second callback to the `then` method.
    - **Example:**
      ```javascript
      let promise = new Promise(function(resolve, reject) {
        reject('Error occurred');
      });

      promise.catch(function(error) {
        console.error(error);
      });

      // Or

      promise.then(null, function(error) {
        console.error(error);
      });
      ```


# Conclusion :

