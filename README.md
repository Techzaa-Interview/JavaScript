# JavaScript Interview Questions

![JavaScript](https://upload.wikimedia.org/wikipedia/commons/thumb/6/6a/JavaScript-logo.png/240px-JavaScript-logo.png)


**Question 1: What is the difference between `null` and `undefined` in JavaScript?**

**Answer:** `null` is an explicitly assigned value that represents the absence of any object value, while `undefined` means that a variable has been declared but has not yet been assigned a value.

---

**Question 2: How would you compare two objects in JavaScript?**

**Answer:** You cannot directly compare two objects in JavaScript using `==` or `===` because they compare object references, not the actual object values. You would need to compare the properties of the objects manually.

---

**Question 3: Explain the concept of prototypal inheritance in JavaScript.**

**Answer:** In JavaScript, objects can inherit properties and methods from other objects. This is achieved through prototypal inheritance, where objects can have a prototype object that serves as a template for the properties and methods of the object.

---

**Question 4: How do you handle errors in JavaScript?**

**Answer:** Errors in JavaScript can be handled using `try`, `catch`, and `finally` blocks. The `try` block contains the code that might throw an error, the `catch` block handles the error if one occurs, and the `finally` block executes code after the try and catch blocks, regardless of whether an error occurred or not.

---

**Question 5: What are closures in JavaScript and how are they used?**

**Answer:** Closures are functions that have access to variables from their containing scope even after the containing function has finished executing. They are used to create private variables and methods in JavaScript.

---

**Question 6: What is the difference between synchronous and asynchronous code in JavaScript?**

**Answer:** Synchronous code is executed sequentially, blocking further execution until the current operation is completed. Asynchronous code allows the program to continue executing other operations while waiting for the asynchronous operation to complete, using callbacks, promises, or async/await.

---

**# Question 7: How does event delegation work in JavaScript?

**Answer:** Event delegation is a technique where a single event listener is attached to a parent element, rather than multiple event listeners being attached to individual child elements. This allows you to manage events on dynamically added elements or reduce the number of event listeners needed.

---

