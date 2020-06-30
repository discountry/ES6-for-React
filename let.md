## let

### Defination

> The let statement declares a block scope local variable, optionally initializing it to a value.

### Syntax

```js
let var1 [= value1] [, var2 [= value2]] [, ..., varN [= valueN]];
```

### Examples

```js
function varTest() {
  var x = 1;
  if (true) {
    var x = 2;  // same variable!
    console.log(x);  // 2
  }
  console.log(x);  // 2
}

function letTest() {
  let x = 1;
  if (true) {
    let x = 2;  // different variable
    console.log(x);  // 2
  }
  console.log(x);  // 1
}
```

### Usage

```jsx
function Title(props) {
  let content = props.content
  return (
    <h1>{content}</h1>
  )
}
```

### References

* [MDN let](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let)