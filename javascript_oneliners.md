# How to reverse String

<details>
  <summary>Click to expand!</summary>
  
  ```Java
    [...'Mohan'].reverse().join('')
  ```
</details>

# VM777:1 Uncaught TypeError: String.prototype.matchAll called with a non-global RegExp argument

<details>
  <summary>"abcssssabcdfdkdfkdabc".matchAll(/ab+/) -- why does this line throws error</summary>
  It was missing global flag
  ```Java
  "abcssssabcdfdkdfkdabc".matchAll(/ab+/g)
  [..."abcssssabcdfdkdfkdabc".matchAll(/ab+/g)]
  ```
</details>

# How to iterate all the div in HTML DOM

<details>
  <summary>let divs = document.getElementsByTagName('div')</summary>
  This avoids the overhead of checking the length of the array. 
  Ensures that the div variable is reassigned to the current item each time around the loop for added convenience.

  ```Java
  let divs = document.getElementsByTagName('div')
  for (let i = 0, div; div = divs[i]; i++) {
    /* Process div in some way */
  }
  ```
</details>

## What are all Array like objects in javascript? Does it support all the Array methods?
1. ArrayLike
  1. arguments
  1. NodeList - document.getElementsById
  1. string
1. They won't support all the Array methods, but we can make use of Function.prototype.call method - to invoke some of Array methods

## Where to find javascript Array document

1. MDN > References > Javascript > Built-in-Objects > Array
1. [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)
