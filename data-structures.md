# Data Structures

- Arrays
- Objects

## Arrays
Arrays are lists of values. These values can be different sort of values. you can store numbers and strings in the same array. Arrays are made with square brackets `[]` and use a comma `,` to seperate each value. The last value doesn't end with a comma.
```js
var arrayVoorbeeld = ["Hey", "Ho", 1];
```
To get select a specific value inside a array you type the array name and it's index between `[]`. The index of an array starts at 0. So `arrayVoorbeeld[1];` will return `"Ho"`.

### Array Methods
Methods are properties that contain contain functions. Methods apply to different values or data structures. An array has multiple methods:
- `.push()`: adds values to the end of an array
- `.pop()`: removes values that are added last to an array
- `.unshift()`: adds values to the start of an array
- `.shift()`: removes values from the start of an array
- `.slice()`: selects the start and ending of an array. The start index is included, the end index not. If you only use one number in the slice, it will start from that index and go on till the end of the array.
- `.indexOf()`: will return the first index of the value between the `()`
- `.lastIndexOf()`: will return the last index of the value between the `()`
- `.concat()`:can glue arrays together similar to the `+` sybol for strings
```js
//push
var sports = ['soccer', 'baseball'];
var total = sports.push('football', 'swimming');

console.log(sports); // ['soccer', 'baseball', 'football', 'swimming']
console.log(total);  // 4

//shift
var a = [1, 2, 3];
var b = a.shift();

console.log(a); // [2, 3]
console.log(b); // 1

//slice
console.log([0, 1, 2, 3, 4,].slice(2, 4)); // [2, 3]

//indexOf
console.log([0, 1, 2, 3, 4,].indexOf(3)); // 2

//concat
var alfa = ['a', 'b', 'c'],
var nummer = [1, 2, 3];

var alfaNummer = alfa.concat( nummer );

console.log(alfaNummer); // ['a', 'b', 'c', 1, 2, 3]
```

## Objects
Object are a handy way to group variables that are related. Objects make your code more readable and DX friendly. Properties within an object exist out of an `key:` and a `value,` like this:
```js
let car = {
  sedan: false,
  "visited countries": ["Nederland", "België", "Germany", "Amsterdam"]
};

console.log(car.sedan);
// → false

console.log(car.windows);
// → undefined

car.windows = false;

console.log(car.windows);
// → false
```
You can use arrays and other objects as properties of an object. You can add new properties to an object by using a dot:`.newProperty`. You can remove properties by using the `delete` keyword. 
```js
let car = {
  sedan: false,
  "visited countries": ["Nederland", "België", "Germany", "Amsterdam"]
};

delete car.sedan;

console.log(car.sedan); 
// → undefined

console.log(sedan in car); 
// → false
```

To view an object's properties you can use the `.keys` method.
```js
console.log(Object.keys({x: 0, y: 0, z: 2}));
// → ["x", "y", "z"]
```

