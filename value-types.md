# Values

JS uses multiple values witch all exist out of bits. Chunks of bits are called values:
- Numbers
- Arithmetic
- Special numbers
- Strings
- Unary operators
- Boolean values
- Logical operators
- Empty values
- Automatic type conversion

## Numbers
Number values are numeric values. Simply just numbers like `8`. You are aloud to use numbers with decimals `8.12` and scientific notations with `e` like this: `2.998e8` this means `2.998 x 10^8 = 299.800.000`

## Arithmetic
The main thing to do with numbers is arithmetic (using multiple numbers to create new numbers). The artithmetic operators are `+`, `-`, `*`, `/` and `%`.
Their usage is quite clear accept for `%`, this gives a rest number. `314 % 100 = 14`.

## Special numbers
There are 3 special numbers in JS. These values are considered numbers, but don't act like it. The numbers are:
- `infinity`
- `-infinity`
- `NaN`

## Strings
Strings are used to represent text and are used between quotes `""` `''`. You can use single or double quotes as long as you begin and end with the same quotes. If you use a backward dash `\` it indicates that the character after it is a special character like a dash `\`, or a tab `\t`. If you write something inside `${}` it's result will be comuted and included in that position. You can add strings to eachother using the `+` arthmetic operator.

## Unary operators
Unary operators are operators that use 1 value. An example of an unary operator is the `typeof` operator. This operator will return what kind of value is placed after it. 
```js
function goeiemorguh() {
  console.log(typeof "Goeiemorguh");
 }
 
 goeiemorguh();
 
 // => string
 ```
 
 ## Boolean values
 Boolean has just 2 values: 
 - `true` or
 - `false`
 
 ## Logical operators
 Logical operators are used to reason about booleans.  There are 3 types of logical operators:
 - `&&` (and)
 - `||` (or)
 - `!` (not)
 
 There is also a ternary operator which uses 3 values:
 - It is written with a `?` and a `:` like this:
```js
console.log(true ? 1 : 2);
// => 1

console.log(false ? 1 : 2);
// => 2
```

 ## Empty values
 There are 2 empty values. They mean the abscence of any value at all, and practically mean the same.
 - `null`
 - `undefined`
 
 ## Automatic type conversion
 If you use two values with eachother which aren't the same sort of value JS will guess what you mean. These "guesses" aren't always logical.
