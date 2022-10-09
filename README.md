### Hi there 👋

## Exercise Wednesday 10/05/2022

```js
function isPalindrome(line) {
  // if number --> string
  // string --> array
  // reverse values
  //  array --> string
  // compare values
  let lineStr = line.toString();
  let strArr = lineStr.split("").reverse().join("");
  return strArr === lineStr ? true : false;

  // Optimize
  //   let lineStr = line.toString()
  // return lineStr.split('').reverse().join('') === lineStr
}
```

## Exercise Wednesday 10/05/2022

```js
// function well(x) {
//   let count = 0;
//   for (let i = 0; i < x.length; i++) {
//     if (x[i] === "good") {
//       count++;
//     }
//   }
//   if (count > 0 && count <= 2) return "Publish!";
//   if (count > 2) return "I smell a series!";
//   return "Fail!";

// Optimize
  const count = x.filter((x) => x === 'good').length
  return count < 1 ? 'Fail!' : count < 3 ? 'Publish!' : 'I smell a series!'
}

```
## Exercise Friday 10/07/2022
```js
import React from 'react';

export class Counter extends React.Component {
  constructor(props) {
    // Your state
    super()
    this.state = {
      counter: 0
    }
    
    this.increment = this.increment.bind(this)
    this.decrement = this.decrement.bind(this)
  }
  
  increment(){
    this.setState({ counter: this.state.counter + 1})
  }
  
  decrement(){
    this.setState({ counter: this.state.counter - 1})
  }
  
  // Your event handlers 
  render() {
    return (
      <div>
        <h1 id="counter">{this.state.counter}</h1>
          <button id="increment" type="button" onClick={this.increment}>
            Decrement
          </button>
          <button id="decrement" type="button" onClick={this.decrement}>
            Increment
          </button>
      </div>
    )
  }
}

```