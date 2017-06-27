# Introduction

## Why I wrote this?

Facebook has just released the v15.5.0 of React.

In this new version, some main functions (e.g. `createClass`) are deprecated.

React supported ES6 syntax since v0.14.*, and Facebook recommends us to use new ES6 syntax to write React App.

But most of us are still stay in the "jQuery Age", we hate new syntax, we hate JSX, and we don't want to change.

Actually, many new syntaxes ES6 standard offer us are quite useful. Especially keywords like `class` `import` and etc. truly enhanced the capabilities of JavaScript. Syntactic sugar like arrow function could save lots of our time.

But at the same time, ES6 JavaScript is much more like a totally different language for newbies. We have to change lots of traditions as well as learn many new keywords we haven't seen.

So, it's very necessary for us to learn ES6 JavaScript before we learn React.

Of course, many of us don't have that much time to go through the whole standard document of ES6. So, I gathered the most important parts of ES6 that we often apply in React, reorganized those key points for saving learners' time.

## Why using ES6+ syntaxes

If you refuse to use ES6 & JSX features, you probabbly have to write React code like this:

```js
var createReactClass = require('create-react-class');

var Greeting = createReactClass({
  render: function() {
    return React.createElement('div', null, 'Hello ' + this.props.name);
  }
});
```

But when using `arrow function` and JSX you are able to refactor above codes in one line:

```js
const Greeting = props => <div>Hello {props.name}</div>
```

## Who should read this?

Newbie who want to learn the newest version of React, but have no idea what ES6 is.

The learner who want to change, learn new things and taste the super power of ES6.

## Packages version

* [react@15.5.4](https://libraries.io/npm/react/15.5.4)
* [react-dom@15.5.4](https://libraries.io/npm/react-dom/15.5.4)
* [redux@3.6.0](https://libraries.io/npm/redux/3.6.0)

## Softwares we use

* [Sublime Text 3](https://www.sublimetext.com/)
