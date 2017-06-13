## Array.prototype.map()

### Defination

> The map() method creates a new array with the results of calling a provided function on every element in the calling array.

### Syntax

```js
var new_array = arr.map(function callback(currentValue, index, array) {
    // Return element for new_array
}[, thisArg])
```

### Examples

```js
var numbers = [1, 5, 10, 15];
var doubles = numbers.map(function(x) {
   return x * 2;
});
// doubles is now [2, 10, 20, 30]
// numbers is still [1, 5, 10, 15]

var numbers = [1, 4, 9];
var roots = numbers.map(Math.sqrt);
// roots is now [1, 2, 3]
// numbers is still [1, 4, 9]
```

### Usage

```jsx
const numbers = [1, 2, 3, 4, 5];
const listItems = numbers.map((number) =>
  <li>{number}</li>
);
```

### References

* [MDN Array.prototype.map()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map)