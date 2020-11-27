# Tutorial: Intro to React

https://reactjs.org/tutorial/tutorial.html

- [ ] https://reactjs.org/docs/hello-world.html

## Before We Start the Tutorial



### What Are We Building?

[Final Result: Tic-Tac-Toe](https://codepen.io/gaearon/pen/gWWZgR?editors=0010)

### Prerequisites

[A re-introduction to JavaScript (JS tutorial) - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript)

[Arrow function expressions - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions)

[Classes - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

[let - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let)

[const - JavaScript | MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const)

## Setup for the Tutorial

### Local Development Environment

:shipit: $ [`npx create-react-app tictactoe`](https://github.com/arafatm/learn-reactjs-tutorial/commit/bcecaf55349d8bf25dc24332bd5dd85983040dcc)

[:ship: b7a4f46](https://github.com/arafatm/learn-reactjs-tutorial/commit/b7a4f46)
Clean `src/` folder to start clean
```bash
rm -rf src/*
```

[:ship: 4cefb50](https://github.com/arafatm/learn-reactjs-tutorial/commit/4cefb50)
initial react files `index.css` & `index.js` in `src/`
```bash
touch src/index.css src/index.js
```

[:ship: 376db93](https://github.com/arafatm/learn-reactjs-tutorial/commit/376db93)
Initial React setup in `index.js`
```react
import React from 'react';
import ReactDOM from 'react-dom';
import './index.css';
```

[:ship: `npm start`](http://localhost:3000/)

### Help, I'm Stuck!

[Where To Get Support – React](https://reactjs.org/community/support.html)

[Reactiflux chat on Discord](https://discord.com/channels/102860784329052160/377580704722190347)

## Overview

### What Is React?

`React.Component` includes a `render` that displays the component and will re-render on an update.

```react
class ShoppingList extends React.Component {
  render() {
    return (
      <div className="shopping-list">
        <h1>Shopping List for {this.props.name}</h1>
        <ul>
          <li>Instagram</li>
          <li>WhatsApp</li>
          <li>Oculus</li>
        </ul>
      </div>
    );
  }
}

// Example usage: <ShoppingList name="Mark" />
```

A Component can also take a `prop`, in this case a `name`.

### Inspecting the Starter Code

[:ship: e030091](https://github.com/arafatm/learn-reactjs-tutorial/commit/e030091)
Initial game setup with Components: `game`, `board`, `square`

[:ship: 100f5e4](https://github.com/arafatm/learn-reactjs-tutorial/commit/100f5e4)
Passing props

```react
class Board extends React.Component {
  renderSquare(i) {
    return <Square value={i} />;
  }
}

class Square extends React.Component {
  render() {
    return (
      <button className="square">
        {this.props.value}
      </button>
    );
  }
}
```

xxx

### Passing Data Through Props

### Making an Interactive Component

### Developer Tools

### Completing the Game

### Lifting State Up

### Why Immutability Is Important

### Function Components

### Taking Turns

### Declaring a Winner

## Adding Time Travel

### Storing a History of Moves

### Lifting State Up, Again

### Showing the Past Moves

### Picking a Key

### Implementing Time Travel

### Wrapping Up
