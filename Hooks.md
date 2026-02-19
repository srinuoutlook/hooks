# useState Hook - Complete Guide

The `useState` hook is one of the fundamental hooks in React, introduced in version 16.8. It allows you to manage state in functional components. Before the introduction of hooks, state management was only possible in class components.

## Basic Usage

To use `useState`, you need to import it from React:

```javascript
import { useState } from 'react';
```

You can then call `useState` within your functional component:

```javascript
const [count, setCount] = useState(0);
```

Here, `count` is the current state value, and `setCount` is a function that updates the state. The initial value of `count` is set to `0`. 

## Updating State

You can update the state by calling the `setCount` function:

```javascript
setCount(count + 1);
```

This will increment `count` by one.

## Multiple State Variables

You can call `useState` multiple times to manage different pieces of state in the same component:

```javascript
const [name, setName] = useState('');
const [age, setAge] = useState(0);
```

## Functional Updates

If the new state is based on the previous state, you can pass a function instead:

```javascript
setCount(prevCount => prevCount + 1);
```

## Conclusion

The `useState` hook is a powerful addition to React that makes state management in functional components more straightforward and efficient. It allows for cleaner code and promotes the use of functional programming concepts in React applications.