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
- closing tags are optional, however it is recommended to use them as their omission may result in unexpected results across different browsers
- elements with no content are called empty elements, an example of which is the ```<br>``` tag which defines a line break
- tags are not case sensitive, however the accepted convention is to use lowercase tags

### Attributes

All HTML elements can make use of attributes, which provide **additional information** about the element.

- always specified in the start tag
- usually come in ```key="value"``` pairs
- it is recommended to use lower case attributes

Common attributes:

|Attribute|Used in|Function|
|---------|-------|--------|
|href|```<a>```|Specifies link address|
|src|```<img>```|Specifies source of content, such as filenames|
|width, height|```<img>```|Specify dimensions|
|alt|```<img>```|Specifies text to be used in cases where image cannot be displayed, such as the use of "screen readers" by visually impaired people|
|style|all tags|Specifies styling of an element|
|lang|```<html>```|Declares language of document|
|title|all tags|Defines tooltip text|

**Note**: In attributes that require quotes, the convention is to use double quotes. However it may be necessary to use a combination of single and double quotes in certain circumstances such as:

```<p title='John "ShotGun" Nelson'>```

or

```<p title="John 'ShotGun' Nelson">```

### Headings

Search engines use headings to **index** the structure and content of a page. ```<h1>``` signifies very important content, with the importance diminishing with each increment in the tag.

- Each HTML heading has a default size which may changed using the font-size CSS property of the style attribute: ```<h1 style="font-size:60px;">Heading 1</h1>```
- The ```<hr>``` tag may be used to create a horizontal rule, representing a thematic break in the content of a page

### Paragraphs

- the screen size will affect how HTML content is rendered
- **whitespace is ignored** within ```<p>``` tags

### Styles

The style attribute controls the style of an element.

This attribute has the following syntax: ```<tagname style="property:value;">```. Property and value refer to CSS.

Some examples:

|Style|Function|Example|
|-----|--------|-------|
|background-color|Defines the background colour|```<body style="background-color:powderblue;">```|
|color|Defines text colour|```<p style="color:red;">This is a paragraph.</p>```|
|font-family|Defines font type|```<p style="font-family:courier;">This is a paragraph.</p>```|
|font-size|Defines font size|```<h1 style="font-size:300%;">This is a heading</h1>```|
|text-align|Defines horizontal text alignment|```<p style="text-align:center;">Centered paragraph.</p>```|

### Formatting

HTML defines special elements for defining text with a special meaning

Examples of formatting tags:

|Formatting tag|Function|
|--------------|--------|
|```<b>```|bold|
|```<strong>```|important|
|```<i>```|italic|
|```<em>```|emphasis|
|```<mark>```|marked/highlighted|
|```<small>```|small|
|```<del>```|deleted|
|```<ins>```|inserted|
|```<sub>```|subscript|
|```<sup>```|superscript|

### Quotation and Citation Elements

|Element|Function|Example|
|-------|--------|-------|
|```<q>```|Short quotations|```<p>WWF's goal is to: <q>Build a future where people live in harmony with nature.</q></p>```|
|```<blockquote>```|Sections quoted from a source|```<blockquote cite="http://www.worldwildlife.org/who/index.html">For 50 years, WWF has been protecting the future of nature</blockquote>```|
|```<abbr>```|Abbreviations|```<abbr title="World Health Organization">WHO</abbr>```|
|```<address>```|Contact information|```<address>Written by John Doe.</address>```|
|```<cite>```|Titles of works|```<cite>The Scream</cite>```|
|```<bdo>```|Override text directions|```<bdo dir="rtl">This text will be written from right to left</bdo>```|

### Comments

Comments can be added to HTML as follows:

```HTML
<!-- Do not display this at the moment
<img border="0" src="pic_trulli.jpg" alt="Trulli">
-->
```

### Colors

HTML colours may be defined using:

- **Predefined Names**

Examples include: __DodgerBlue__ and __Tomato__

```<p style="background-color:Tomato;">Lorem ipsum...</p>```

- **RGB**

rgb(red, green, blue), where each parameter defines the intensity from 0 to 255

```<h1 style="background-color:rgb(255, 0, 0);">rgb(255, 0, 0)</h1>```

- **Hexadecimal**

\#rrggbb, where rr, gg and bb represent hexadecimal values from 00 to ff

```<h1 style="background-color:#ff0000;">#ff0000</h1>```

- **HSL**

hsl(hue, saturation, lightness), where hue is a degree on the colour wheel (0 to 360), saturation is a percentage ranging from a shade of grey at 0% to the full colour at 100% and lightness is a percentage ranging from 0% which is black to 100% which is white (50% would be neither light nor dark)

```<h1 style="background-color:hsl(0, 100%, 50%);">hsl(0, 100%, 50%)</h1>```

- **RGBA**

An extension of RGB to include an alpha value which controls transparency (from 0.0 which is fully transparent to 1.0 which is opaque)

```<h1 style="background-color:rgba(255, 99, 71, 0);">rgba(255, 99, 71, 0)</h1>```

- **HSLA**

An extension of HSLA, analagous to RBGA.

```<h1 style="background-color:hsla(9, 100%, 64%, 0);">hsla(9, 100%, 64%, 0)</h1>```

### CSS

**Cascading Style Sheets** describe how HRML elements are to be displayed.

CSS may be added in the following ways:

- **Inline CSS**

Making use of the style attribute

- **Internal CSS**

Making use of the ```<style>``` tag in the head section of the document

```HTML
<head>
<style>
body {background-color: powderblue;}
h1   {color: blue;}
p    {color: red;}
</style>
</head>
```

- **External CSS**

Making use of the ```<link>``` tag in the head section of the document

```HTML
<link rel="stylesheet" href="styles.css">
```

or 

```HTML
<link rel="stylesheet" href="https://www.w3schools.com/html/styles.css">
```

Depending on where the stylesheet being linked is located

**Common CSS Properties**

|Property|Function|Example|
|--------|--------|-------|
|border|Defines a border around an element|```p {border: 1px solid powderblue;} ```|
|padding|Defines a space between the border and the contents of an element, such as text|```p {border: 1px solid powderblue; padding: 30px;}```|
|margin|Defines a space around the border of an element|```p {border: 1px solid powderblue; margin: 50px;}```|


CSS can be selectively applied to elements as follows:

- Applying to a type of element

```CSS
p {
  border: 1px solid powderblue;
}
```

- Applying to a specific element

Making use of the **id** attribute (note that ids must be unique)

```HTML
<p id="p01">I am different</p>
```

```CSS
#p01 {
  color: blue;
}
```

- Applying to a group of elements

Making use of the **class** attribute

```HTML
<p class="error">I am different</p>
```

```CSS
p.error {
  color: red;
}
```
