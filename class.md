## class

### Defination

> The class declaration creates a new class with a given name using prototype-based inheritance.

### Syntax

```js
class name [extends] {
  // class body
}
```

### Examples

```js
class Polygon {
  constructor(height, width) {
    this.name = 'Polygon';
    this.height = height;
    this.width = width;
  }
}

class Square extends Polygon {
  constructor(length) {
    super(length, length);
    this.name = 'Square';
  }
}
```

### Usage

Example from [react](https://facebook.github.io/react/docs/state-and-lifecycle.html#adding-local-state-to-a-class).

```jsx
class Clock extends React.Component {
  constructor(props) {
    super(props);
    this.state = {date: new Date()};
  }

  render() {
    return (
      <div>
        <h1>Hello, world!</h1>
        <h2>It is {this.state.date.toLocaleTimeString()}.</h2>
      </div>
    );
  }
}
```

### References

* [MDN class](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/class)