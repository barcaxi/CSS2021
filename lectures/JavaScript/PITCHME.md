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

[@fa[external-link]](https://github.com/noucampdotorgCSS2021/javascript/blob/main/exercises/JavaScriptEx1.md)


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

[@fa[external-link]](https://github.com/noucampdotorgCSS2021/javascript/blob/main/exercises/JavaScriptEx1.md)



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

[@fa[external-link]](https://github.com/noucampdotorgCSS2021/javascript/blob/main/exercises/JavaScriptEx2.md)


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

[@fa[external-link]](https://github.com/noucampdotorgCSS2021/javascript/blob/main/exercises/JavaScriptEx3.md)





---
@title[Event Handling]
### Event Handling

@ul[](true)
- We should keep our JavaScript & HTML @size[1.5em](separate)
- HTML should be in a `.html` file
- JavaScript should be in a `.js` file
- This adheres to the @size[1.5em](Separation of Concerns Principle)
@ulend

---
@title[Event Handling]
### Event Handling

Event Handling Steps

@ol[](true)
- Identify HTML element that causes event (e.g. `<a>`)
- Identify the event type (e.g. `onclick`)
- Write event handler function in JavaScript file
@olend


@ul[](true)
- Let's revisit our hyperlink example...
@ulend

---
@title[Event Handling]
### Event Handling

`FirstEventV2.html` (HTML only):

```html
<!DOCTYPE html>
<html>
<head>
<script src="FirstEventV2.js"></script>
</head>
<body>
<a id="fcb" href="www.fcbarcelona.com">FCB</a>
</body>
</html>
```
@[4](our JavaScript code script.js is loaded here)
@[4,7](our hyperlink with an id attribute)
@[*]()


---
@title[Event Handling]
### Event Handling

`FirstEventV2.js` (JavaScript only):

```javascript
window.onload = function()
{
  var aTag = document.getElementById("fcb"); // 1.

  aTag.onclick = function() // 2.
  {
    alert("about to enter the FC Barcelona website"); // 3.
  }
}
```
@[1,2,9](when the window loads run this code)
@[1,2,9,3](1. Get a reference to the element that causes event)
@[1,2,9,3,5](2. Identify the event type)
@[1,2,9,3,5,6-8](3. Event handler code)
@[*]()

[@fa[external-link]](http://localhost/javascript/FirstEventV2.html)

---
@title[Event Handling]
### More Events

@ul[](true)
- `onclick` - mouse clicks an element
- `onload` - a page or image is finished loading
- `onblur` - an element loses focus
- `onfocus` - an element gets focus
- `onchange` - change in a text box or dropdown box
- `onmouseout` - mouse is moved off an element
- `onmouseover` - mouse is moved over an element
- `onselect` - text is selected
- `onsubmit` - the submit button is clicked
- See more event info [here](http://www.w3schools.com/jsref/dom_obj_event.asp)
@ulend


---
@title[Exercise 3]
### Exercise 3 - Event Handling Part 2

[@fa[external-link]](https://github.com/noucampdotorgCSS2021/javascript/blob/main/exercises/JavaScriptEx3.md)


---
@title[Exercise 4 5]
### Exercise 3 - Event Handling Part 3 & 4

[@fa[external-link]](https://github.com/noucampdotorgCSS2021/javascript/blob/main/exercises/JavaScriptEx3.md)



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
- Event Handling
- **Creating DOM Elements**

@olend


---
@title[Creating DOM Elements]
### Creating DOM Elements

3 methods are used to create new DOM elements

@ul[](true)
- ``createElement()``
- ``appendChild()``
- ``createTextNode()``
- Let's see an example...
@ulend


---
@title[Creating DOM Elements]
### Creating DOM Elements

Consider the HTML:

```html
<ul id="myList">
 <li>Rihanna</li>
 <li>Lady Gaga</li>
</ul>
```

![img](/images/createElement1.png)


---
@title[Creating DOM Elements]
### Creating DOM Elements

@ul[](true)
- You can create new HTML elements and add them to the DOM.
- Let's add a new `<li>` element for _Miley Cyrus_
- Two steps to do this:
@ulend
@ol[](true)
- Create the element
- Add it to the DOM...
@olend


---
@title[Creating DOM Elements]
### 1. Create the Element

```javascript
var newElement = document.createElement("li");
var myText = document.createTextNode("Miley Cyrus");
newElement.appendChild(myText);
```
@[1](create the li element)
@[1,2](create the element text node)
@[1,2,3](add the text node to the element)

@ul[](true)
- Other elements that have text nodes are `<p>`, `<h1>`, `<a>`, etc.
- See [createElement()](https://developer.mozilla.org/en-US/docs/Web/API/Document/createElement), [appendChild()](https://developer.mozilla.org/en-US/docs/Web/API/Node/appendChild), [createTextNode()](https://developer.mozilla.org/en-US/docs/Web/API/Document/createTextNode)
@ulend

---

![img](/images/createElement2.png)


- `<li>` element for Miley Cyrus created but unattached...

---
@title[Creating DOM Elements]
### 2. Add the element to DOM

```javascript
var newElement = document.createElement("li");
var myText = document.createTextNode("Miley Cyrus");
newElement.appendChild(myText);

var myList = document.getElementById("myList");
myList.appendChild(newElement);
```
@[5](get a reference to the ul)
@[5,6](add our newElement to the ul)
@[*]()

---

![img](/images/createElement3.png)

- `<li>` element for Miley Cyrus added 

---
@title[Creating DOM Elements]
### Creating DOM Elements

Let's try adding a new anchor element to a `<div>` container:

```html
<div id="myLinks">
</div>
```

---
@title[Creating DOM Elements]
### 1. Create the Element

```javascript
var newElement = document.createElement("a");
var myText = document.createTextNode("Miley Cyrus");
newElement.setAttribute("href","www.mileycyrus.com/");
newElement.appendChild(myText);
```
@[1](create the a element)
@[1,2](create the element text node)
@[1,2,3](set element attribute ahref)
@[1,2,3,4](add the text node to the element)

![img](/images/nelly1.png)

---
@title[Creating DOM Elements]
### 2. Add the element to DOM

```javascript
var newElement = document.createElement("a");
var myText = document.createTextNode("Miley Cyrus");
newElement.setAttribute("href","www.mileycyrus.com/");
newElement.appendChild(myText);

var myLinks = document.getElementById("myLinks");
myLinks.appendChild(newElement);
```
@[6](get a reference to the div)
@[6,7](add our newElement to the div)
@[*]()

![img](/images/nelly2.png)

---
@title[Exercise 4]
### Exercise 4 - DOM Manipulation

[@fa[external-link]](https://github.com/noucampdotorgCSS2021/javascript/blob/main/exercises/JavaScriptEx4.md)




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
- Event Handling
- Creating DOM Elements
- **Form Validation**

@olend

---
@title[Form Validation]
### Form Validation

![img](/images/aform.png)
<!-- ![img](images/aform.png) -->

---
@title[Form Validation]
### Form Validation

The 2 most important things forms have are:
@ol[](true)
- the values of the form elements
- the events that happen when you use a form
@olend

---
@title[Form Validation]
### Form Validation

A simple form:

![img](/images/aform.png)
<!-- ![img](images/aform.png) -->

and it's HTML code...

---
@title[Form Validation]
### Form Validation

```html
<h1>Registration Page</h1>

<form id="myFormId" method="POST" action="process.php">
   Email
   <input id="emailId" name="email" type="text" />
   Password
   <input id="passwordId" name="password" type="password" />

   <input value="Register" type="submit" />
</form>
```
@[3,10](form element)
@[3,10,4-7](labels, textbox & password textbox)
@[3,10,4-7,9](submit button)

---
@title[Form Validation]
### Form Validation

```html
<h1>Registration Page</h1>

<form id="myFormId" method="POST" action="process.php">
   Email
   <input id="emailId" name="email" type="text" />
   Password
   <input id="passwordId" name="password" type="password" />

   <input value="Register" type="submit" />
</form>
```

JavaScript can access the `<form>` by it's `id` attribute:
```javascript
var form = document.getElementById("myFormId");
```

---
@title[Form Validation]
### Form Validation

```html
<h1>Registration Page</h1>

<form id="myFormId" method="POST" action="process.php">
   Email
   <input id="emailId" name="email" type="text" />
   Password
   <input id="passwordId" name="password" type="password" />

   <input value="Register" type="submit" />
</form>
```

JavaScript can access form elements by their `id` attribute:
```javascript
var email = document.getElementById("emailId");
```

---
@title[Form Validation]
### Form Validation

Let's see @size[1.5em](values) and common @size[1.5em](events) for some form elements like:
@ul[](true)
- text boxes
- radio & check buttons
- dropdown boxes
- submit buttons
- These are the basics you need to know.
@ulend


---
@title[Form Validation]
### Form Validation

**Text box**
```html
<input id="emailId" name="email" type="text" />
```
**Property:** `value`
```javascript
var email=document.getElementById("emailId").value;
```
**Events:** `onblur`, `onfocus`, `onchange`, `onkeypress`, `onkeydown`, `onkeyup`

[@fa[external-link]](http://localhost/javascript/form_textbox.html)

---
@title[Form Validation]
### Form Validation

**Check & Radio buttons**
```html
<input id="agree" name="agree" type="checkbox">Click to agree</input>
```
**Property:** `checked`
```javascript
if(document.getElementById("agree").checked)
   alert("Thanks");
else
   alert("You must agree to continue");
```
**Events:** `onclick`, `onchange`

[@fa[external-link]](http://localhost/javascript/form_checkbox.html)


---
@title[Form Validation]

**Dropdown box**
```html
<select id="colour" name="colour">
  <option value="Red">Red</option>
  <option value="Green">Green</option>
</select>
```
**Properties:** `value`, `text`, `length`, `selectedIndex`, `options[]`

```javascript
// print the text from the selected option
var select=document.getElementById("colour");
alert(select.options[select.selectedIndex].text);
```
**Events:** `onchange`,

[@fa[external-link]](http://localhost/javascript/form_select.html)


---
@title[Form Validation]
<!-- ### Form Validation -->

**FORM element**
```html
<form id="myFormId" method="POST" action="process.php">
   ...
   ...
   <input type="submit" value="Register" />
</form>
```
**Properties:** None

**Events:** `onsubmit` is called when submit button is clicked

```javascript
// capture form being submitted
document.getElementById("myFormId").onsubmit=function()
{
   // validate form here
}
```

---
@title[Form Validation]
### Form Validation

Let's do some form validation

![img](/images/validate1.png)
<!-- ![img](images/validate1.png) -->

---
```html
<form id="myFormId" method="POST" action="process.php">
   Email: <input id="emailId" name="email" type="text" />
   Password: <input id="passwordId" name="password" type="password" />
   <input value="Register" type="submit" />
</form>
<p id="errorMsg"></p>
```
@[1-5](The form)
@[1-5,6](a div for error messages)

---

```javascript
window.onload = function(){
   document.getElementById("myFormId").onsubmit=function()  {
      // check email is provided
      if(document.getElementById("emailId").value=="") {
         document.getElementById("errorMsg").innerHTML="You MUST provide an email address";
         return false; //NB stops form submission
      } 
      else {
         document.getElementById("errorMsg").innerHTML="";
         return true;
      }
   }
}
```
@[1,13](when the page loads)
@[1,13,2,12](when the submit button is clicked...)
@[1,13,2,12,4,7,8,11](is email textbox empty?)
@[1,13,2,12,4,7,8,11,5,6](display a error message and ...)
@[1,13,2,12,4,7,8,11,5,6](stop form being posted)
@[1,13,2,12,4,7,8,11,5,6,9,10](else clear messages and post form)
@[*]()


---
@title[Exercise 5]
### Exercise 5 - Form Validation

[@fa[external-link]](https://github.com/noucampdotorgCSS2021/javascript/blob/main/exercises/JavaScriptEx5.md)



---?color=black
@ulend
@title[The End]

@snap[west headline text-white span-70]
JavaScript
@snapend

@snap[south-west]
@fa[envelope-o pad-right-icon]@css[contact-email](thomas.devine@lyit.ie)
@snapend

