### Hi there 👋
## Exercise Wednesday 10/05/2022

```js
function isPalindrome(line) {
// if number --> string 
// string --> array
// reverse values
//  array --> string
// compare values
  let lineStr = line.toString()
  let strArr = lineStr.split('').reverse().join('')
  return strArr === lineStr ? true : false
  
  // Optimize
  //   let lineStr = line.toString()
  // return lineStr.split('').reverse().join('') === lineStr
  
}
```