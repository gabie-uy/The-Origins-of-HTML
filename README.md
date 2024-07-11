# The Origins of HTML

 All my notes, resources, and the activities I made to learn HTML from Codédex

## Elements - elemental.html

An ``element`` usually consists of an opening tag, the content, and a closing tag. A tag is enclosed in angle brackets.

    <p>Hello World!</p>

The ``<p>`` paragraph element tells the browser that the content inside is "paragraph" text.

The ``<body>`` element defines an HTML document's "body" and it's where any content that we want to display to the user will be held:

    <body> opening tag begins the "body".
    <p>👋 I'm a new web developer!</p> is some text in a paragraph element.
    </body> closing tag ends the "body".

***There can only be one ``<body>`` element in an HTML file.***

**TWO SPACES** is recommended for indentations.

## Heading - newspaper.html

Suppose we want to add a headline to our website that displays a news article. Here's how we would do it using a ``<h1>`` heading element and a ``<p>`` paragraph element.

There are six levels of section headings, from ``<h1>`` to ``<h6>``

***Note: Only one ``<h1>`` element should be used in a .html file.***

## Line Break

Pressing enter won't do us any good because HTML ignores multiple spaces and line breaks within elements.

Line break is ``<br>``

A self-closing tag doesn't need to be closed manually by a closing tag (i.e., it does not have a separate closing ``</tag>``). The break tag is the first one we have encountered.

## Text Formatting - corporate.html

- ``<b>`` element to bold text.
- ``<i>`` element to italicize text.
- ``<u>`` element to underline text.
- ``<s>`` element to strikethrough text.

        <b>This text is using bold formatting.</b><br>
        <i>This text is using italics formatting.</i><br>
        <u>This text is using underline formatting.</u><br>
        <s>This text is using strikethrough formatting.</s><br>

***Note: The ``<b>`` element is just for bolding text stylistically; HTML also has a ``<strong>`` element used to convey that the content inside is important, as well as styling it to be bold.***

## Lists - chef.html

**Two types of HTML lists:**

1. ``<ul>`` Unordered lists - Known as bullet points
2. ``<ol>`` Ordered lists - Known as numbered lists

``li`` means list items that is used for both types

## Links - pet.html

``<a>`` anchor element! This link tag allows us to add a hyperlink to a piece of text. Let's see how we can do this:

<a href="https://archive.org/web">Internet Archive</a>

An ``href``, or **hyperlink reference**, is a reference or pointer to another website that is linked in our HTML. When the text “Internet Archive” is clicked, the HTML will redirect to that site, which in our case, is https://archive.org/web!

***Note: This can also be used to point to an email or phone number using a ``mailto:``, ``tel:``, or ``sms:`` parameter, respectively.***

## Images

- The ``<img>`` image element is another self-closing tag, so it doesn't have a closing tag.
- ``src`` attribute, which stands for “source”, specifies the file path of the image.
- ``"https://i.redd.it/5unn16axx1v81.jpg"`` is the image path.

## HTML Structure - blueprint.html

**MUST-HAVES**
- ``<!DOCTYPE html>`` is the document type declaration that appears at the top of a .html file and tells the browser that our file is written in HTML5. This is used with a <html> element containing all the code processed on the page.

*Notice how the ``<!DOCTYPE html>`` doesn’t have a closing tag, while ``<html>`` does.*

***Note: All HTML files must start with a ``<!DOCTYPE html>`` declaration and the ``<html>`` element.***

**Inside ``<html>``, there should be two elements:**

``<head>``: This contains all the info for your browser that's not visible on the page.

``<body>``: This contains all of the content that you will end up seeing on the page.
The <title> element goes in the <head> and assigns text to the tab in our browser.

     <!DOCTYPE html>
     <html>
       <head>
         <title>Codédex | Start your coding adventure ⋆˙⟡</title>
       </head>
       <body>
         Code goes here
       </body>
     </html>

## Parents & Children - family_tree.html

Most individual elements can be parents with one or more child elements.

Here are some relationships:

- ``<head>`` and ``<body>`` are children of ``<html>``.
- ``<title>`` is the child of ``<head>``.
- ``<i>`` is child of ``<p>`` and grandkid of ``<body>``.

Elements can also be **siblings** if they share a direct parent element. Take this unordered list, for instance:

    <body>
      <ul>
        <li>🍄 Mario</li>
        <li>🐢 Luigi</li>
      </ul>
    </body>

The two ``<li>`` elements are siblings because both are children of the same parent, the ``<ul>`` element.
















