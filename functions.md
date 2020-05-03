# Functions
Functions are a very important part of JS. Functions are bundles of pieces of logic that you can reuse. 

## Functions 101
A very basic function and the call of a function looks like this:
```js
function basics() {
  console.log("Basic function");
}

basics();
```

## Function Expression
Function expressions are basically functions inside a variable. The difference between a normal function an a function expression is that function expressions aren't hoisted to the top and need a `;` after it. Function expressions look like this:
```js
var basics = {
  console.log("Basic function");
};

basics();
```

## Arrow Functions
Arrow functions are functions that don't need the function keyword and instead use an arrow `=>` like this:
```js
var arrowFunction = (a) => {
  return a + 1;
};
```

With one parameter you don't need the brackets `()`:
```js
var arrowFunction = a => {
  return a + 1;
};
```
With only one line of code you can leave out the other brackets `{}` and the return keyword:
```js
var nameFunction = a => a + 1;
```

