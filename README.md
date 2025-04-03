# JavaScript Cheat Sheet 2025

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
