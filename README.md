# Basic JavaScript Cheat Sheet 2025

## Syntax


<details>
<summary>Arithmetic</summary>

<br/>

```sh
console.log(1 + 1); // One plus one, prints: 2
console.log(5 * 5); // 5 multiplied by 5, prints 25
console.log(10 / 2); // 10 divided by 2, prints 5
```

<br/>

Increment
```sh
let age = 20;
age++;

console.log(age); // Prints 21
```

<br/>

Decrement
```sh
let age = 20;
age--;

console.log(age); // Prints 19
```

<br/>

Parentheses
```sh
console.log(5 + (2 * 2)); // Prints 9
```


<br/>

</details>


<details>
<summary>Comments</summary>

<br/>

Comments allow you to add notes to your code, without effecting the code itself.

```sh
// This is a single line comment
 ```
```sh
/*
This is a multi line comment
*/
 ```

<br/>

</details>


<details>
<summary>Conditional Statements</summary>

<br/>

Conditional statements allow you to execute code according to defined conditions. The conditions are executed as either or.

<br/>

Examples of basic if statements
```sh
if (1 == 1) {
    console.log("If condition was true"); // Will be printed
}
if (1) {
    console.log("If condition was true"); // Will be printed
}
if (1 < 2 ) {
    console.log("If condition was true");  // Will be printed
}
 ```

<br/>

Examples of basic if and else if statements
```sh
if (1 < 2 ) {
    console.log("If condition was true"); // Will be printed
} else if ( 1 < 3) {
    console.log("Else if condition was true"); // Wont be printed
}
 ```
```sh
if (1 == 2 ) {
    console.log("If condition was true"); // Wont be printed
} else if ( 1 < 3) {
    console.log("Else if condition was true"); // Will be printed
}
 ```

<br/>

Examples of basic if, else if and else statements
```sh
if (1 > 2 ) {
    console.log("If condition was true"); // Wont be printed
} else if ( 1 > 3) {
    console.log("1st else if condition was true"); // Wont be printed
} else if ( 1 > 4) {
    console.log("2nd else if condition was true"); // Wont be printed
} else {
    console.log("Else condition was true"); // Will be printed
}
 ```
```sh
if (1 > 2 ) {
    console.log("If condition was true"); // Wont be printed
} else if ( 1 > 3) {
    console.log("1st else if condition was true"); // Wont be printed
} else if ( 1 == 1) {
    console.log("2nd else if condition was true"); // Will be printed
} else {
    console.log("Else condition was true"); // Wont be printed
}
 ```
```sh
if (1 == 1 ) {
    console.log("If condition was true"); // Will be printed
} else if ( 1 > 3) {
    console.log("1st else if condition was true"); // Wont be printed
} else if ( 1 > 4) {
    console.log("2nd else if condition was true"); // Wont be printed
} else {
    console.log("Else condition was true"); // Wont be printed
}
```

<br/>

Conditional statements can be nested inside one another

```sh
if (1 == 1) {
    console.log("If condition was true"); // Will be printed
    if (1 > 2) {
        console.log("1st nested if condition was true");
    } else if (1 < 2) {
        console.log("2nd nested if condition was true"); // Will be printed
    }
} else {
    console.log("Else condition was true");
}
```

<br/>

</details>


<details>
<summary>Data Structures</summary>

<br/>

Variables store single values, but data structures store multiple values and enables the organisation of these values.

Array
```sh
let cats = ["Gary", "Frank", "Shona", "Steve", "Wendy"];
 ```

<br/>

Object
```sh
let cat = { name: "Gary", age: 12 };
 ```

<br/>

Object Array
```sh
let cats = [
    { id: 1, name: "Gary", age: 12 },
    { id: 2, name: "Frank", age: 18 },
];
```

<br/>

Map
```sh
const cats = new Map([
    ["Gary", 12],
    ["Frank", 18],
]);
```


<br/>

</details>


<details>
<summary>Functions</summary>

<br/>

JavaScript code is built around functions. Functions can be used to the organise code, silo functionality making the code easer to read and debug, and return values/functionality.

```sh
function functionA() {
    console.log("Function A executed");
}

functionA(); // Call the function
```
```sh
function functionA() {
    console.log("Function A executed");
}

function functionB() {
    console.log("Function B executed"); // Not printed because the function is never called
}

functionA(); // Call the function
```
<br/>

In the example below, one function is called which then triggers two other functions.

```sh
function functionA() {
    console.log("Function A executed");
}

function functionB() {
    console.log("Function B executed");
}

function mainFunction() {
    functionA();
    functionB();
}

mainFunction();
```

<br/>

```sh
function functionA(x, y) {
    return x * y;
}

let coordinates = functionA(2, 5);

console.log(coordinates); // Prints: 10
```


<br/>

</details>



<details>
<summary>Loops</summary>

<br/>

Loops have a number of use cases. For example, a loop can be used to "loop"/repeat lines of code until a condition is met, or to minimise file size by reducing repetitive code. The loops below show different ways to print the numbers 1 to 10.

<br/>

"for" loop, execute this code "for" as long as a condition is true.

```sh
for (let i = 1; i <= 10; i++) {
    console.log(i);
}
 ```

<br/>

"while" loop, execute this code "while" a condition is true.

```sh
let i = 1;

while (i <= 10) {
    console.log(i);
    i++;
}

 ```

<br/>

</details>


<details>
<summary>Print</summary>

<br/>

Printing allows you to print messages to a console. Developers can use it for debugging.

```sh
console.log("cat");
 ```
```sh
console.log(45);
 ```
```sh
console.log(5 + 5); // Prints "10" to the console
 ```
```sh
console.log("5 + 5"); // Prints "5 + 5" to the console
 ```

<br/>

console.table can be used to print in a table format
```sh
let cats = [
    { id: 1, name: "Gary", age: 12 },
    { id: 2, name: "Frank", age: 18 },
];

console.table(cats);
```

<br/>

A console.log combined with JSON.stringify will print the items in JSON format
```sh
let cats = [
    { id: 1, name: "Gary", age: 12 },
    { id: 2, name: "Frank", age: 18 },
];

console.log(JSON.stringify(cats, null, 2));
```


<br/>

</details>


<details>
<summary>Variables</summary>

<br/>

Variables can be declared as either a "var", "let" or "const". Using "let" and "const" is good modern practice. A "let" should be used for a variable whose value will change. A "const" (constant) should be used for variables that will not change in value.

<br/>

const variable examples
```sh
const cat = "Steve";
const age = 22;
const cost = 22.75;
const storeOpen = false;
 ```

<br/>

let variable examples
```sh
let cat = "Steve";
let age = 22;
let cost = 22.75;
let storeOpen = false;
 ```

</details>
