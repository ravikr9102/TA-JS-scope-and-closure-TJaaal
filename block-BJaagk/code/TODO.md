1. Convert the function below into different forms of function expression.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}

// Answer
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
```

2. Write Function Declaration or Function Expression next to the function.

```js
function percentage(marks, total) {
  return (marks * 100) / total;
}
// Function Declaration
```

```js
let percentage = function percentage(marks, total) {
  return (marks * 100) / total;
};
// Function Expression
```

```js
let percentage = function (marks, total) {
  return (marks * 100) / total;
};
// Function Expression
```

```js
let percentage = (marks, total) => {
  return (marks * 100) / total;
};
// Function Expression
```

```js
let percentage = (marks, total) => (marks * 100) / total;
// Function Expression
```

3. Why is a function definition an expression in JavaScript? Give one example of function expression.

//  A function expression is very similar to and has almost the same syntax as a function declaration.The main difference between a function expression and a function declaration is the function name, which can be omitted in function expressions to create anonymous functions.

Example: (Function Expression)
let percentage = function (marks, total) {
  return (marks * 100) / total;
};


4. Why is a function call an expression in JavaScript?

// A function call expression is used to execute a specified function with the provided arguments. If the function being called is overloaded, the compiler will attempt to match the argument types with the function parameter types. If there are no matching function declarations, a compile-time error will be raised.

5. Write VALID and INVALID next to each example below with the reason.

```js
function add(a, b) {
  return a + b;
}

let five = add(2, 3); // Valid
five = add; // Valid 
five = five(10, 11); // Valid 
five = function () {
  return "Hello";
}; // Valid
```

6. What is the difference between function definition and function call? Explain with an example.

Using a function to do a particular task any point in program is called as function call. So the difference between the function and function call is, A function is procedure to achieve a particular result while function call is using this function to achive that task.

function add(){ // Defination

}

add(); // Call


7. What is the similarities between function definition and function call?

// Function Defination is an expression (function is an object)
// Function Call is an expression (function call always return a value)

8. Is the code below valid or invalid. Explain with reason.

```js
function hello() {
  console.log("Hello World!");
}

hello.user = "Sam"; // valid
```

9. What is higher order function explain with an example.

// That accepts a function defination
// that returns a function defination

function add(cb){ // HOF
  cb()
}
function add(){ // HOF
  function main(){}
  return main
}

10. Explain what is callback function. Why you can pass a function inside a function?

// Because function is an expression in JS we can pass a function inside another function