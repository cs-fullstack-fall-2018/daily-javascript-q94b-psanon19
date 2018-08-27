# daily-javascript-q94b

You have the following code:

```javascript
<body>
<div id="main">
    <p>paragraph 1</p>
    <p class="target">paragraph 2</p>
    <p>content 2</p>
    <p class="target">Some more content here</p>
    <p>paragraph 3</p>
</div>
<div>
    <p class="target">
        <span>paragraph 4</span>
    <div class="target">content 4</div>
    <p class="target">Some more content here</p>
    </p>
</div>

<script>
    var items = document.getElementsByTagName("div")[1].getElementsByClassName("target");
    for (var i = 0; i < items.length; i++) {
        var child = document.createElement("p");
        var child2 = document.createTextNode("Some text");
        child.setAttribute("style", "color:red; border: 1px solid green;");
        child.appendChild(child2);
        items[i].appendChild(child);
    }
</script>
</body>
```

How many elements will be red with a green border?

Choose the correct answer

1) 1
2) 2
3) 3
4) 4

***The Answer is 1***
