# Declaring Variables

There are three ways to declare variables in Javascript:

``` javascript
var one = 1;
let two = 2;
const three = 3;
```

## var
This variable function scoped meaning it is available throughout the entire function. For example, if it a var variable was assigned in line 10, it would exist in line 1. It is also mutable

## let
Also a mutable variable however it is confined within the block in which it was defined. Always defined within {}.

## const
Similar to let in that it is also block scoped, however it is not mutable.

```javascript
const obj = { a: 3 };
obj = { b: 5 } // not allowed
```

```javascript
const obj = { a: 3 };
obj.a = 5;  // allowed
```
a const means the reference is protected from reassignment. The value is not immutable though and can change. The values inside of obj can change, but odj itself cannot.

## When to use what
const by default
let in loops
and there is no need for var anymore


# Data Types
Numbers in Javascript are always float.

## Checking Type
typeof -> returns string type of the data type primitive
instanceof -> returns a Boolean of if a value matches the data type

## Types can change
``` javascript
let x = 'something'
x = 1

x = 1 + 'hello' // output:'1hello'
```

Output will be a string because Javascript will find a common ground between two values, and coerce them into a string

``` javascript
let x = 0 == ''; // true, type coerced

let x = 0 === ''; // false, type respected
```

The first example is true because Javascript coerces them to be comparable and thus 0 as a number has the same value as an empty string.
The triple equal sign does not coerce them to be the same type, therefore 0 as a number is not equal to an empty string.


