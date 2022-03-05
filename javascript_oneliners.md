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
