# Airbnb - Good practices collection

* <https://github.com/airbnb/javascript>
* <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/from>

## Arrays

* **Array Creation**: Use the literal syntax

```javascript
const items = [];
```

* **Adding items**: Use `push(item)` instead of direct assignment

```javascript
const items = [];
items.push("first");
items.push("second");
items.push("third");
```

* **Copying arrays**: Use array spread operator

```javascript
const items = [];
items.push("first");
items.push("second");
items.push("third");

//Shallow copy
const itemsCopy = [...items];
```

* **Convert at iterable object to an array**: Use spread operator

```javascript
const divElements = document.querySelectorAll("div");

//Shallow copy
const nodes = [...divElements];
```

* **Converting an array-like object to an array**: - Use `Array.from`

```javascript
const arrLike = { 0: "foo", 1: "bar", 2: "baz", length: 3 };
const arr = Array.from(arrLike);
```

* **Mapping over iterables**: Use `Array.from` instead of spread, because it avoids creating an intermediate array. `Array.from(arrayLike, mapFn)`

```javascript
const mapOverIterablesResult = Array.from(iterableItems, mappingFunction);
```

* **Array method callback function** - Use `return` statement if more than oneline in function body.

```javascript
const squares = [1, 2, 3].map((x) => x * x);

[[0, 1], [2, 3], [4, 5]].reduce((acc, item, index) => {
  console.log(acc + "-" + item + "-" + index)  
  const flatten = acc.concat(item);
  return flatten;
});


filteredItems = inbox.filter((msg) => {
  const { subject, author } = msg;
  if (subject === 'Mockingbird') {
    return author === 'Harper Lee';
  }

  return false;
});
```

* **Array declaration and initialization** - Use line breaks after open and before close array brackets if An array has multiple lines

```javascript
const arr = [
  [0, 1],
  [2, 3],
  [4, 5], //Note the trailing comma
];

const objectInArray = [
  {
    id: 1,
  },
  {
    id: 2,//Note the trailing comma
  },//Note the trailing comma
];

const numberInArray = [1, 2];
```
