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
