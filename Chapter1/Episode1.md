# Introduction

### What actually is javascript and why was it invented?

**Javascript is basically a programming language which can run on a browser.**

So in the early 1990's most websites had static content which could only be read or viewed like articles and documentations. Web pages containing information about a historical event or personal hobbies which can only be read but not engaged with. Images were all static, which means there was no click to zoom functionality, no image sliders or carousels to allow users to scroll through multiple images by clicking previous or next navigation buttons.
These webpages were built only on HTML and CSS. <br><br>
HTML defined the structure and content of the website and CSS was used to provide beauty to the web pages. To add interactivity to these more or less dead web pages, was the the very reason javascript was invented.<br>

### How did javascript increase user engagement and interactivity?

- Earlier if an HTML page contained forms, the form validation would happen in the server side i.e. checking if an email was in correct format or password met a certain criteria needed a server side round trip. With the introduction of javascript the client side validation became possible, giving instant feedback to user and preventing form submission for invalid input.
- Javascript also responds to user interactions such as button clicks, mouse movements. It does it by attaching event listeners to the elements on the page which wait for specific events to trigger a function.
- We discussed that earlier browsers were built entirely on HTML can CSS only. HTML is a static markup language useful for structuring the content. Therefore there was no room for dynamic content updates without reloading the entire page. Earlier if updates were to be shown, the server had to generate a completely new HTML page and send it back to the browser. This new HTML page replaced the current HTML page and this whole process would cause a reload. Every interaction requiring server communication meant reloading the entire page, which includes clicking a hyperlink, submitting a form, to fetch new content like updated news or something.<br><br>
How did javascript solve this issue? <br><br>
1)Dynamic DOM Manipulation : Javascript allows direct modification of parts of web page by manipulating the DOM. What is DOM though?<br>
DOM is --> Document (the whole HTML or XML document) Object (each element in the HTML file `<p>`,`<h1>`,`<div>` is treated as object) and Model (The document is represented as a hierarchical model or tree structure, where each element in the HTML file is a node in the tree, with child nodes representing nested elements.)<br>
When a browser loads an HTML doc, it parses the HTML file and creates a DOM tree which represents the structure of the document.
This DOM is provided by web browsers to allow us (developers) to interact with and manipulte each element of the HTML file we are working with. Whether it be changing text written inside a `<p>` or changing the style of paragraph itself. It can also be adding a new `<p>` tag inside an already existing `<p>` tag or triggering a function when someone clicks or hovers or performs any other event on that paragraph.<br>
Basically the DOM is a bridge between javascript and HTML, giving javascript the access to all the elements present in the body of HTML<br>
Note that these HTML elements are provided to us as objects, and like every object they have certain properties and methods. For a `<div>` we have : <br>
Properties : style, id, className, children (elements inside the div tag) etc.
Methods : appendChild() : to add another node inside the div, remove() : to remove an existing node, addEventListener() : to attach event listeners like 'click', 'scroll' etc.<br>
**So, now dynamic updates are possible in the HTML file without needing a server side trip, thus preventing the page from reloading.**