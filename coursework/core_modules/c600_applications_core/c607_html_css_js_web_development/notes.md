|![W3Schools](w3.png)| **HTML, CSS, and Javascript for Web Developers** |
|----------------------------------|--------------------:|

Course started: 21/01/2019

## HTML

### Introduction

HTML (Hyper Text Markup Language) is the standard markup language for web pages.

- describes **structure** of web pages
- elements are the bulding blocks of HTML
- elements are represented by tags
- tags label pieces of content
- **broswers render content** of page from tags

Simple example:

```HTML
<!DOCTYPE html>
<html>
<head>
<title>Page Title</title>
</head>
<body>

<h1>My First Heading</h1>
<p>My first paragraph.</p>

</body>
</html>
```

Explanation of tags:

|Tag|Function|
|---|--------|
|```<!DOCTYPE html>```|Defines document to be HTML5|
|```<html>```|Root element of an HTML page|
|```<head>```|Contains meta information about the document|
|```<title>```|Specifies document title|
|```<body>```|Contains visible page content|
|```<h1>```|Large heading|
|```<p>```|Paragraph|

### Basics

- heading tags range from ```<h1>```(largest) to ```<h6>```(smallest)
- links make use of the ```<a>``` tag which is used as follows: ```<a href="https://www.google.com/">Google</a>```
- images are defined with ```<img>```, which is structured as follows: ```<img src="w3schools.jpg" alt="W3Schools.com" width="104" height="142">```
- buttons may be defined with ```<button>```
- lists in html come in two variants, ```<ol>``` for numbered lists and ```<ul>``` for bullet point lists. both make use of the ```<li>``` tag to define list elements
