## import

### Defination

> The import statement is used to import functions, objects or primitives that have been exported from an external module, another script, etc.

### Syntax

```js
import defaultMember from "module-name";
import * as name from "module-name";
import { member } from "module-name";
import { member as alias } from "module-name";
import { member1 , member2 } from "module-name";
import { member1 , member2 as alias2 , [...] } from "module-name";
import defaultMember, { member [ , [...] ] } from "module-name";
import defaultMember, * as name from "module-name";
import "module-name";
```

### Examples

```js
// --file.js--
function getJSON(url, callback) {
  let xhr = new XMLHttpRequest();
  xhr.onload = function () { 
    callback(this.responseText) 
  };
  xhr.open('GET', url, true);
  xhr.send();
}

export function getUsefulContents(url, callback) {
  getJSON(url, data => callback(JSON.parse(data)));
}

// --main.js--
import { getUsefulContents } from 'file';
getUsefulContents('http://www.example.com', data => {
  doSomethingUseful(data);
});
```

### Usage

```jsx
// --Todo.js--
import React from 'react';

const Todo = ({content}) => (
  <li><a href="/#">{content}</a></li>
  )

export default Todo;
// --TodoList.js--
import React from 'react';
import Todo from './Todo';

const TodoList = ({ todos }) => (
    <ul>
        {todos.map((todo) => (
            <Todo key={todo.id} content={todo.content} />
        ))}
    </ul>
);

export default TodoList;
```

### References

* [MDN import](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/import)