# javascript-notes

* javascript <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide>
* react <https://reactjs.org/docs/getting-started.html#learn-react>

## Tips - Mozilla documentation

* What is the topic?

```javascript
items = []
document.querySelectorAll("h1").forEach(node => items.push(node.innerText))
topics = items.slice()
topics
```

* What are the subtopics?

```javascript
items = []
document.querySelectorAll("h2").forEach(node => items.push(node.innerText))
topics = items.slice(2,-4)
topics
```

* What does each subtopic covers?

```javascript
items = []
document.querySelectorAll("h3 a").forEach(node => items.push(node.innerText))
topics = items.slice(2,-4)
topics
```

* Any h4 level points? => **currently no**

```javascript
items = []
document.querySelectorAll("h4").forEach(node => items.push(node.innerText))
topics = items.slice()
topics
```
items = []
document.querySelectorAll("div dl").forEach(node => items.push(node.innerText))
topics = items.slice(2,-4)
topics


## Mozilla - Javascript reference

<https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object>

```javascript
const headings = [...document.querySelectorAll("div dl dt")]
const description =  [...document.querySelectorAll("div dl dd")]
if (headings.length === description.length) {
    methodDescription = headings.map(function(e, i) {
  return [e, description[i]];
});
}
<!-- contentEnd = "Full support"
methodDescription.indexOf()
console.log(methodDescription) -->
methodDescription.forEach(item => console.log(item[0].innerText + "-" + item[1].innerText))
```

items =[...document.querySelectorAll("h3")]
items.forEach(node => console.log(node.innerText))
