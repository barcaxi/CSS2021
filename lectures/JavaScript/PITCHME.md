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


---
@title[Contents]
### Contents

@ol[](false)
- What is JavaScript?
- Three Web Layers
- Separation of Concerns
- Hello World
- **Code Fundamentals**

@olend


---
@title[Code Fundamentals]
### Code Fundamentals

@ol[](false)
- Variables
- Template Strings
- Arrays
- Conditional statement
- Loops
- Functions

@olend


---
@title[Variables]
### Variables


```javascript
var name;                
name="Bob"; 
alert(name);

var age = 21; 
var pi = 3.14159265;

var found = true; 

var fname = "tom";
var lname = "jones";
var fullname = fname + " " + lname;
console.log(fullname);
```
@[1]
@[1,2]
@[1,2,3]
@[5]
@[6]
@[8]
@[10,11]
@[10,11,12]
@[10,11,12,13]

---
@title[Template Strings]
### Template Strings

@ul[](false)
- You can embed expressions within strings
- For example...
@ulend

```javascript
var name;                
name="Bob"; 
console.log(`Hello ${name}`);

var fname = "tom";
var lname = "jones";
console.log(`${fname} ${lname}`);
```
@[1-3]()
@[5-7]()
@[*]()


---

@title[Arrays]
### Arrays

```javascript
var names = []; 
names[0]="tom"; 
names[1]="john";	

var names = ["tom","john"];

var lotto = [1,2,3,4,5,6];

var mixed = [1,"two",3.14];
```
@[1]()
@[1-3]()
@[1-3,5]()
@[7]()
@[9]()


---
@title[if statement]
### if statement

```javascript
var age=17;
if(age<18) 
{   
  alert("too young to vote"); 
} 

var name="tom";
if(name=="tom") 
{   
  alert(`hello ${name}`); 
} 
else 
{   
  alert("hello stranger") 
}
```
@[1-5]()
@[7-15]()

---
@title[for loop]
### for loop

```javascript
var numbers=[1,2,3,4]; 

for(var i=0;i<numbers.length;i++)
  numbers[i]=numbers[i]*2; 
```

---
@title[while loop]
### while loop

```javascript
var numbers=[1,2,3,4]; 

var i=0;
while(i<numbers.length)
{   
  console.log(numbers[i]);   
  i++; 
}
```

---
@title[do while loop]
### do while loop


```javascript
var numbers=[1,2,3,4]; 

do 
{   
  alert(numbers[i]);   
  i++; 
} while(i<numbers.length);
```


---
@title[Functions]
### Functions

```javascript
function printText() {
  alert("hello"); 
}

function printText(text) {   
  alert(text); 
} 

function sqr(number) {   
  return number*number;
}

printText();
printText("hello");
console.log(sqr(3));
```
@[1-3,13]()
@[5-7,14]()
@[9-11,15]()

---
@title[Exercise 2]
### Do Exercise 1 - Part 2

[@fa[external-link]](https://github.com/noucampdotorgCSS2021/javascript/blob/master/exercises/JavaScriptEx1.md)



---
@title[Contents]
### Contents

@ol[](false)
- What is JavaScript?
- Three Web Layers
- Separation of Concerns
- Hello World
- Code Fundamentals
- **The DOM**

@olend

---
@title[The DOM]

### DOM

@ul[list-bullets-black](true)
- The @size[1.5em](Document Object Model)
- A browser stores HTML code as a hierarchy of objects in the DOM
- Each HTML element (tag) in a web page is an object in the DOM
- JavaScript can access these objects...
@ulend

---
@title[The DOM]

### DOM

```html
<!-- DOMhtml.html -->
<html>
<head>
<title>DOM JavaScript</title>
</head>
<body>
<h1>DOM JavaScript</h1>
<p>Read JavaScript articles from
<a href="http://www.danwebb.net/">Dan Webb</a>,
<a href="http://www.quirksmode.org/">PPK</a> and
<a href="http://adactio.com/">Jeremy Keith</a>.
</p>
</body>
</html>
```
[@fa[external-link]](http://localhost/javascript/DOMhtml.html)

---
@title[The DOM]

### DOM

![img](/images/dom2.png)

---
@title[The DOM]
### DOM nodes

@ul[list-bullets-black](true)
- The _document node_ (aka root node) is the top node of the tree
- Each HTML element is an _element node_
- HTML content is represented by _text nodes_ and _attribute nodes_
- Anything not inside angled brackets is a text node
- The value of the text node for the `<title>` element is `DOM JavaScript`
@ulend

---
@title[The DOM]

### DOM

```html
<!-- DOMhtml.html -->
<html>
<head>
<title>DOM JavaScript</title>
</head>
<body>
<h1>DOM JavaScript</h1>
<p>Read JavaScript articles from
<a href="http://www.danwebb.net/">Dan Webb</a>,
<a href="http://www.quirksmode.org/">PPK</a> and
<a href="http://adactio.com/">Jeremy Keith</a>.
</p>
</body>
</html>
```
[@fa[external-link]](http://localhost/javascript/DOMhtml.html)


---
@title[The DOM]
### DOM

![img](/images/dom3.png)


---
@title[The DOM]
### DOM Attribute nodes

@ul[list-bullets-black](false)
- Element attributes have their own node called an _attribute node_
- The anchor elements, ``<a>``, could be visualised as:
@ulend

![img](/images/dom5.png)

---
@title[The DOM]
### Accessing DOM Nodes

JavaScript functions you need to know to access and manipulate the DOM:

@ul[list-bullets-black](true)
- `getElementById()`
- `getAttribute()`
- `setAttribute()`
- `getElementsByTagName()`
- `querySelector()`
@ulend


---
@title[The DOM]
### Accessing the DOM

```html
<title id="title">DOM JavaScript</title>
```

@ul[list-bullets-black](true)
- The most direct way to access an element is via its ``id`` attribute
- The ``id`` attribute can be added to any element
- Each ``id`` must be unique within the page
- The ``getElementById()`` method is then used...
@ulend


---
@title[The DOM]
### Accessing the DOM

`- DOMhtml.html -`
```html
<html>
<head>
<title>DOM JavaScript</title>
</head>
<body>
<h1>DOM JavaScript</h1>
<p>Read JavaScript articles from
<a href="http://www.danwebb.net/">Dan Webb</a>,
<a href="http://www.quirksmode.org/">PPK</a> and
<a href="http://adactio.com/">Jeremy Keith</a>.
</p>
</body>
</html>
```

@[6](Let's change the ``<h1>`` heading text...)


---
@title[The DOM]
### Accessing the DOM

`- DOMhtml.html -`
```html
<html>
<head><title>DOM JavaScript</title></head>
<body>
<h1 id="heading1">DOM JavaScript</h1>

<p>Read JavaScript articles from
<a href="http://www.danwebb.net/">Dan Webb</a>,
<a href="http://www.quirksmode.org/">PPK</a> and
<a href="http://adactio.com/">Jeremy Keith</a>.
</p>

<script type="text/javascript" src="DOMhtml.js"></script>
</body>
</html>
```
@[4](Add an ``id`` to the ``<h1>`` tag)
@[4,12](add a link to a new JavaScript file)
@[*]()


---
@title[The DOM]
### Accessing the DOM

```javascript
// DOMhtml.js

var h1 = document.getElementById("heading1");
console.log(h1.innerHTML);
h1.innerHTML="DOM JavaScript II";
```
@[3](Use ``getElementById()`` to get a reference ``h1`` to the element)
@[3,4](Use the ``h1`` reference to get the innerHTML property)
@[3,4,5](Use the ``h1`` reference to change the innerHTML property)
@[*]()

[@fa[external-link]](http://localhost/javascript/DOM1-Solution.html)


---
@title[The DOM]
### Accessing node attributes values

```html
<a href="http://www.lyit.ie">LYIT</a>
```

@ul[list-bullets-black](true)
- You can get and set the value of any node attribute
- e.g. let's get the ``href`` of the an ``<a>`` tag...
@ulend


---
@title[The DOM]
### Accessing node attributes values

`- DOMhtml.html -`
```html
<html>
<head><title>DOM JavaScript</title></head>
<body>
<h1 id="heading1">DOM JavaScript</h1>
<p>Read JavaScript articles from
<a id="danwebb" href="http://www.danwebb.net/">Dan Webb</a>,
<a href="http://www.quirksmode.org/">PPK</a> and
<a href="http://adactio.com/">Jeremy Keith</a>.
</p>
<script type="text/javascript" src="DOMhtml.js"></script>
</body>
</html>
```
@[6](add an ``id`` to the ``<a>`` tag)
@[6,10](add our JavaScipt code in DOMhtml.js)
@[*]()

---
@title[The DOM]
### Accessing node attributes values


```javascript
// DOMhtml.js

var a1 = document.getElementById("danwebb");
console.log(a1.getAttribute("href"));
```
@[3](get a reference to the `<a>` element)
@[3,4](Use ``getAttribute()`` to access an attribute)
@[*]()

[@fa[external-link]](http://localhost/javascript/DOM1-Solution.html)

---
@title[The DOM]
### Changing a node attribute value

```html
<a href="http://www.lyit.ie">LYIT</a>
```

@ul[list-bullets-black](true)
- Attributes can be added or changed too
- e.g. let's change the URL of the first ``<a>`` tag...
@ulend


---
@title[The DOM]
### Changing a node attribute value

`- DOMhtml.html -`
```html
<html>
<head><title>DOM JavaScript</title></head>
<body>
<h1 id="heading1">DOM JavaScript</h1>
<p>Read JavaScript articles from
<a id="danwebb" href="http://www.danwebb.net/">Dan Webb</a>,
<a href="http://www.quirksmode.org/">PPK</a> and
<a href="http://adactio.com/">Jeremy Keith</a>.
</p>
<script type="text/javascript" src="DOMhtml.js"></script>
</body>
</html>
```
@[6](let's change this ``href`` value)
@[*]()

---
@title[The DOM]
### Changing a node attribute value

```javascript
// DOMhtml.js

var a1 = document.getElementById("danwebb");
a1.setAttribute("href","http://www.rte.ie/");
```
@[3](get a reference to the `<a>` element)
@[3,4](Use ``setAttribute()`` to change/add an attribute)
@[*]()


[@fa[external-link]](http://localhost/javascript/DOM1-Solution.html)

---
@title[Exercise 2]
### Do Exercise 2 - The DOM

[@fa[external-link]](https://github.com/noucampdotorgCSS2021/javascript/blob/master/exercises/JavaScriptEx2.md)


---
@title[Contents]
### Contents

@ol[](false)
- What is JavaScript?
- Three Web Layers
- Separation of Concerns
- Hello World
- Code Fundamentals
- The DOM
- **Event Handling**

@olend

---
@title[Events]
<!-- ### Events -->

@size[1.5em](Events) are:

@ul[](true)
- clicking a hyperlink
- clicking a button
- selecting a value in a dropdown box
- scrolling
- changing focus
- typing a value into a form field
- a page finished loading
- etc.
@ulend


---
@title[Event Handling]
### Event Handling

@ul[](true)
- An @size[1.5em](event handler) is a function that's bound to an @size[1.5em](event) that happens a node in the DOM
- The function is called automatically when the event happens to the node
- An example...
@ulend 

---
@title[Event Handling]
### Event Handling

A hyperlink: [FC Barcelona](http://www.fcbarcelona.com)

@ul[](true)
- Let's handle a user @size[1.5em](clicking) a hyperlink
- The browser generates an @size[1.5em](onclick) event
- Normally the browser will respond to that click by going to the URL specified
- Before this happens, we'll write an @size[1.5em](event handler) to respond to the event first
@ulend


---
@title[Event Handling]
### Event Handling

`FirstEvent.html`
```html
<!DOCTYPE html>
<html>
<body>
<a href="www.fcbarcelona.com">FCB</a>
</body>
</html>
```


@ul[](true)
- Let's capture the `onclick` event...
@ulend

---
@title[Event Handling]
### Event Handling

`FirstEvent.html`
```html
<!DOCTYPE html>
<html>
<body>
<a href="www.fcbarcelona.com" onclick="msg()">FCB</a>
</body>
</html>
```
@[4](onclick event is an attribute added to anchor tag)
@[4](we'll call an event handler function called msg())
@[*]

@ul[](true)
- Let's add `msg()` event handler for `onclick` event...
@ulend


---
@title[Event Handling]
### Event Handling

```html
<!DOCTYPE html>
<html>
<head>
<script type="text/javascript">
  function msg() {
    alert("about to enter the FC Barcelona website");
  }
</script>
</head>
<body>
<a href="www.fcbarcelona.com" onclick="msg()">FCB</a>
</body>
</html>
```
@[3,4,8,9](SCRIPT tag inside HEAD tag)
@[3,4,8,9,5-7](msg() function is the event handler)
@[*]

[@fa[external-link]](http://localhost/javascript/FirstEvent.html)


---
@title[Exercise 3]
### Do Exercise 3 - Event Handling Part 1

[@fa[external-link]](https://github.com/noucampdotorgCSS2021/javascript/blob/master/exercises/JavaScriptEx3.md)



<!-- FOR TUESDAY BELOW -->






---?color=black
@ulend
@title[The End]

@snap[west headline text-white span-70]
JavaScript
@snapend

@snap[south-west]
@fa[envelope-o pad-right-icon]@css[contact-email](thomas.devine@lyit.ie)
@snapend

