# React-101

## What is React.js? - A front-end library created by Facebook. Specifically for the UI.

### Why would you use React.js?
It's flexible, and creates dynamic maintainable components for web applications. Code can be used through multiple files.

### What are components?
They are like JavaScript functions. They accept “props” and return React elements describing what should appear on the screen. One of the building blocks of React.

### What is JSX?
Syntax extension to JavaScript. Appears like a mix of HTML and returns plain JS elements. 

### What are props?
A way to rewrite usuable features. Props are arguments passed into React components. Props stand for properties. React Props are like function arguments in JavaScript and attributes in HTML.

To send props into a component, use the same syntax as HTML attributes"

### What is state?
State is a built-in React object that is used to contain data or information about the component. Allows us to manage change in data in an app.

### What are the differences btw/ functional and class based components?
A functional component is just a plain JavaScript function which accepts props as an argument and returns a React element.

### Give an example of a functional and class based component?
Functional components are basic JavaScript functions. These are typically arrow functions but can also be created with the regular function keyword.
Sometimes referred to as “dumb” or “stateless” components as they simply accept data and display them in some form; that is they are mainly responsible for rendering UI.

React lifecycle methods (for example, componentDidMount) cannot be used in functional components.
There is no render method used in functional components.
These are mainly responsible for UI and are typically presentational only (For example, a Button component).
Functional components can accept and use props.
Functional components should be favored if you do not need to make use of React state.
Class components make use of ES6 class and extend the Component class in React.
Sometimes called “smart” or “stateful” components as they tend to implement logic and state.
React lifecycle methods can be used inside class components (for example, componentDidMount).
You pass props down to class components and access them with this.props"

```
"CLASS - 
class ClassHelloWorld extends React.Component {
    render() {
      return <h1>Hello, World</h1>;
    }
}   

FUNCTIONAL - 
const FunctionHelloWorld = function () {
    return <h1>Hello, World</h1>;
};"
```
### What are React Hooks?
React Hooks let developers use state and other React features without writing a class. 

### How does useState work?
useState works by letting you add React state to function components.

### Give an example of useState?
```
import React, { useState } from 'react';

function Example() {
  // Declare a new state variable, which we'll call ""count""
  const [count, setCount] = useState(0);

  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}"
```

### What is the Virtual DOM?
A virtual DOM object is a representation of a DOM object, like a lightweight copy. It has the same properties as a real DOM object, but it lacks the real power to directly change what’s on the screen.

### What is two way data binding and one way data flow? How does this relate to react?
Two way data binding means that UI fields are bound to model data dynamically such that when a UI field changes, the model data changes with it. So if using two-way data binding, you always have the same data in Model and View.
One way data flow means that the model is the single source of truth. Only the model has the effect is that data always flows in a single direction, which makes it easier to understand.
