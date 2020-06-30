## export

### Defination

> The export statement is used to export functions, objects or primitives from a given file (or module).

### Syntax

```js
export { name1, name2, …, nameN };
export { variable1 as name1, variable2 as name2, …, nameN };
export let name1, name2, …, nameN; // also var
export let name1 = …, name2 = …, …, nameN; // also var, const

export default expression;
export default function (…) { … } // also class, function*
export default function name1(…) { … } // also class, function*
export { name1 as default, … };

export * from …;
export { name1, name2, …, nameN } from …;
export { import1 as name1, import2 as name2, …, nameN } from …;
```

### Examples

```js
// module "my-module.js"
function cube(x) {
  return x * x * x;
}
const foo = Math.PI + Math.SQRT2;
export { cube, foo };
// module "my-module.js"
export default function cube(x) {
  return x * x * x;
}
```

### Usage

```jsx
import React from 'react';

export const ADD_TODO = 'ADD_TODO';

export const addTodo = (content) => ({
    type: actionType,
    content
});

const App = () => {
    return (
        <div>
            App
        </div>
    );
};

export default App;
```

### References

* [MDN export](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/export)