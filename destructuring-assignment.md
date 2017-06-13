## Destructuring assignment

### Defination

> The destructuring assignment syntax is a JavaScript expression that makes it possible to unpack values from arrays, or properties from objects, into distinct variables.

### Syntax

```js
var a, b, rest;
[a, b] = [10, 20];
console.log(a); // 10
console.log(b); // 20

[a, b, ...rest] = [10, 20, 30, 40, 50];
console.log(a); // 10
console.log(b); // 20
console.log(rest); // [30, 40, 50]

({a, b} = {a: 10, b: 20});
console.log(a); // 10
console.log(b); // 20

// Stage 3 proposal
({a, b, ...rest} = {a: 10, b: 20, c: 30, d: 40});
```

### Examples

```js
// Basic variable assignment
var foo = ['one', 'two', 'three'];

var [one, two, three] = foo;
console.log(one); // "one"
console.log(two); // "two"
console.log(three); // "three"
// Assignment separate from declaration
var a, b;

[a, b] = [1, 2];
console.log(a); // 1
console.log(b); // 2
```

### Usage

```jsx
const Todo = ({ content, onClick, completed }) => (
    <li>
        <div className="view">
            <input onChange={onClick} className="toggle" type="checkbox" checked={completed ? 'checked' : ''} />
            <label href="/#">{content}</label>
        </div>
    </li> 
);
```

### References

* [MDN Destructuring assignment](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Destructuring_assignment)