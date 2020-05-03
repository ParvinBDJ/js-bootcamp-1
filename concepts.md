# Concepts

## Scopes
A scope is the current context of execution. This means that the scope determines the accessibility of variables. There are 3 different kind of scopes:
- The Global scope
- The Local scope
- The Block scope

### Global Scope
The global scope is the scope that surrounds the entire file. Bindings that are defined outside a functional scope are in the global scope. It is best practice to keep the global scope clean. Too many global variables will eventually cause bugs if you aren't carefull.
```js
var globalVariable = "This is global";
```

### Local/Function Scope
If you create a function you also create a function/local scope within it. Every variable you create inside a function will only be visible inside that function. You can also overwrite global variables inside a local scope. This won't overwrite the value of the global variable.
```js
var globalVariable = "This is global";

function createLocalScope() {
  var localVariable = "This variable is only visible inside this function";
}
```

### Block Scope
The block scope is a bit of a strange scope. A block scope is created within the brackets of a loop. A variable created with var is only visible within a local scope. This doesn't apply to the block scope. A variable created with var will be visible outside the block scope. However a variable declared with the let keyword will only be visible inside the block scope. 
```js
var globalVariable = "This is global";

function createLocalScope() {
  var localVariable = "This variable is only visible inside this function";
}

for (let i=0; i<10; i++) {
  // This is inside a block scope
}
```

## Hoisting
The easiest, but not completely accurate, way of explaining hoisting is saying that the variable declarations (with var) and function are placed at the top of the file. In reality hoisting consists of 2 fases: 
1. Creation fase
2. Execution fase

The most important part of the creation fase (for my mental model) is the creation of the variables, but they don't get the value assigned yet.
In the execution fase the code will be read line for line. The values will be assigned here to the var variables.

## Closures
JS uses closures. This means that functions can see variables outside of it's own scope, but the global scope can't see variables that are declared within a local scope.

