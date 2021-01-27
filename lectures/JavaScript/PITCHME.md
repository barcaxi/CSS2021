---?color=black
@title[Title]

@snap[west headline text-white span-70]
JavaScript
@snapend

@snap[south-west]
@fa[envelope-o pad-right-icon]@css[contact-email](thomas.devine@lyit.ie)
@snapend


---
@title[Contents]
### Contents

@ol[](false)
- **What is JavaScript?**

@olend


---
@title[What is Express?]

### What is JavaScript?

@ul[list-bullets-black](true)
- It's a programming language
- The most popular language in the world ~ w3schools.com
- Runs mostly on @size[1.5em](web browsers)
- Web browsers can run JavaScript code
- It's an interpreted language
- It makes web pages interactive

@ulend


---
@title[Contents]
### Contents

@ol[](false)
- What is JavaScript?
- **Three Web Layers**

@olend

---
@title[Three Layers of the Web]
### Three Layers of the Web

@ul[list-bullets-black](true)
- Use *HTML* to produce documents with content 
- Use *Cascading Style Sheets* (CSS) to style that content
- but HTML and CSS are static 
- *JavaScript* can make the content interactive
@ulend


---
@title[Contents]
### Contents

@ol[](false)
- What is JavaScript?
- Three Web Layers
- **Separation of Concerns**

@olend


---
@title[Separation of Concerns]

### Separation of Concerns

@ul[list-bullets-black](true)
- Web designers mix HTML, CSS, and JavaScript in web pages
- @size[1.5em](Don't do this)
- A web page does three fundamental things:
  - it describes the *content* of the page
  - it specifies the *presentation* of that content
  - it controls the *behaviour* of that content
- Keeping these 3 things separate is the principle known as the *separation of concerns*
- Good web developers follow this principle

@ulend

---
@title[Separation of Concerns]

### Why separate?

@ul[list-bullets-black](true)
- It makes it easier to @size[1.5em](reuse) code in future projects
- It @size[1.5em](reduces) the amount of @size[1.5em](duplicate) code you end up writing
- It makes it easier to find and fix problems now and in the future
- It allows you to cater for the different ways people access your content
@ulend

---
@title[Contents]
### Contents

@ol[](false)
- What is JavaScript?
- Three Web Layers
- Separation of Concerns
- **Hello World**

@olend

---
@title[Hello JavaScript World]

### Hello World

`- FirstJS.html -`
```html

<!doctype html>
<html>
<head>
<title>First JavaScript</title>
<script type="text/javascript">
  alert("hello,world!");
  console.log("hello, console!");
</script>
</head>  

<body>
...
</body>
</html>
```
@[6,9](script tag placeholder for JavaScript code)
@[6,9,7,8](alert and console.log)
@[*]()

[@fa[external-link]](http://localhost/javascript/FirstJS.html)

---
@title[Hello JavaScript World]

### Hello World v2

`- SecondJS.html -`
```html

<!doctype html>
<html>
<head>
<title>Second JavaScript</title>
<script type="text/javascript" src="example.js"></script>
</head>  
<body>
Now you see me...
</body>
</html>
```
@[6](load example.js script)

[@fa[external-link]](http://localhost/javascript/SecondJS.html)

---
@title[Hello JavaScript World]

### Hello World v2

```javascript
// example.js
alert("hello,world!");
console.log("hello, console!");
```

[@fa[external-link]](http://localhost/javascript/SecondJS.html)


---
@title[Exercise 1]
### Do Exercise 1 - Part 1

[@fa[external-link]](https://github.com/noucampdotorgCSS2021/javascript/blob/master/exercises/JavaScriptEx1.md)



---?color=black
@ulend
@title[The End]

@snap[west headline text-white span-70]
JavaScript
@snapend

@snap[south-west]
@fa[envelope-o pad-right-icon]@css[contact-email](thomas.devine@lyit.ie)
@snapend

