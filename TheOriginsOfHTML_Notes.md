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

An ``href``, or **hyperlink reference**, is a reference or pointer to another website that is linked in our HTML. When the text “Internet Archive” is clicked, the HTML will redirect to that site, which in our case, is https://archive.org/web

***Note: This can also be used to point to an email or phone number using a ``mailto:``, ``tel:``, or ``sms:`` parameter, respectively.***

## Images

- The ``<img>`` image element is another self-closing tag, so it doesn't have a closing tag.
- ``src`` attribute, which stands for “source”, specifies the file path of the image.
- ``"https://i.redd.it/5unn16axx1v81.jpg"`` is the image path.

## HTML Structure - blueprint.html

### MUST-HAVES

``<!DOCTYPE html>`` is the document type declaration that appears at the top of a .html file and tells the browser that our file is written in HTML5. This is used with a ``<html>`` element containing all the code processed on the page.

*Notice how the ``<!DOCTYPE html>`` doesn’t have a closing tag, while ``<html>`` does.*

***Note: All HTML files must start with a ``<!DOCTYPE html>`` declaration and the ``<html>`` element.***

**Inside ``<html>``, there should be two elements:**

``<head>``: This contains all the info for your browser that's not visible on the page.

``<body>``: This contains all of the content that you will end up seeing on the page.
The ``<title>`` element goes in the ``<head>`` and assigns text to the tab in our browser.

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

## Comments - craigslists.html

Everything surrounded by the ``<!--`` and ``-->`` comment markers is ignored and not rendered on the browser:

    <!-- I am a comment. -->
    <p>And I'm not a comment!</p>

## In-Line vs. Multi-line''

### In-Line

    <p>This text is visible. <!-- But this is not. --></p>

### *Multi-Line**

    <!--
      This is also a comment.
    -->

## Attributes - wiki_article.html

**Attributes** are additional settings that we can use to customize an element.

They are usually name/value pairs, like ``name="value"``, where the name and value are separated by an equals sign:

    <element name="value">Content</element>

The ``name`` indicates the attribute we are setting for our element.
The ``"value"`` for our attribute is surrounded by ``"`` double quotes.

If we want to use **lowercase letters** instead:

    <ol type="a">
      <li>Power ⚡</li>
      <li>Courage 🔥</li>
      <li>Wisdom 🦉</li>
    </ol>

Or, if want to use **Roman numerals**:

    <ol type="i">
      <li>Power ⚡</li>
      <li>Courage 🔥</li>
      <li>Wisdom 🦉</li>
    </ol>

For uppercase list item types for letters and Roman numerals, use type="A" and type="I", respectively.

### Attributes in ``<img>``

    <img alt="8-bit sprite of person using a laptop" src="https://www.codedex.io/images/tier1.png">

- The ``<img>`` element uses the ``src`` attribute to specify the file path of an image.
- The ``alt`` text is displayed instead! This allows assistive devices to read our text and describe the image.

### Attributes in ``<a>``

    <a href="https://www.codedex.io/">Codédex.io</a>
    <a href="https://www.codedex.io/" target="_blank">Codédex.io</a>

- The ``href`` attribute is where we add a URL that can be visited when the hyperlinked text is clicked.
- We can also use the ``target`` attribute and set it to ``"_blank"`` to visit the URL on a separate tab on our browser:

## Classes and IDs - lorem_ipsum.html

``class`` and ``id`` are used for **labeling** elements.

An element can be assigned multiple class values in the form of a **space-separated list**:

    <p class="first-value second-value third-value">Hello, World</p>

Each element can only have one ``id`` value with no spaces. Every ``id`` value should be unique in the entire page:

    <p id="value">Hello, World</p>

Additionally, ``id`` can be *used to link to another part of the same page*, such as the heading! This can be matched with an ``<a>`` anchor element's ``href`` attribute via a ``#`` hashtag symbol, followed by the identifier used for the ``id``:

    <a href="#medellin">Link to Medellín</a>
    
    <h2 class="city" id="medellin">Medellín 🇨🇴</h2>

Lastly, where only one ``id`` can be assigned to a single element, a ``class`` can be assigned to many:

    <h2 class="city" id="medellin">Medellín 🇨🇴</h2>
    <h2 class="city" id="libson">Lisbon 🇵🇹</h2>
    <h2 class="city" id="bali">Bali 🇮🇩</h2>

The values for the ``class`` and ``id`` attributes must always be lowercase. If their name is made of multiple words, they should be separated by dashes ``-``

***Note: A good way to remember class vs id is... there can be multiple students in a class, but each student should have an unique id. 💡***

## Division

``<div>`` is a way to create sections for a page

The ``<div>`` element is kind of like a generic container with no particular meaning. This element and the ``class`` and ``id`` attributes can go hand in hand.

The ``<div>`` element is used to group content and be labeled by the ``class`` and ``id`` attributes.

    <div class="page-section" id="about-me">
        <h2>About Me</h2>
        <p>Ness is an aspiring web developer!</p>
      </div>
      
    <div class="page-section" id="social-media">
      <h2>Social:</h2>
        <ul>
          <li>GitHub</li>
          <li>Twitter</li>
          <li>LinkedIn</li>
      </ul>
    </div>

## Style Attribute

We can apply a ``style`` attribute to any HTML element to stylize certain aspects of that element, such as what color the text should be:

    <p>
      Roses are <span style="color:red;">red</span>.<br />
      Violets are <span style="color:blue;">blue</span>.
    </p>

This attribute uses a *special syntax* where a style is made of a property (i.e., color) and a value (red), separated by a  ``:`` colon. Multiple styles can be applied to a single element, but they must be separated by a ``;`` semi-colon.

    <p>
      Roses are <span style="color:red; text-decoration:underline;">red</span>.<br />
      Violets are <span style="color:blue; text-decoration:underline;">blue</span>.
    </p>

Alternatively, the ``<style>`` element can be used in the ``<head>`` to style our elements in the ``<body>``.

    <!DOCTYPE html>
    <html>
      <head>
        <style>
          ... Styles for elements go here
        </style>
      </head>
      <body>
        ... Elements go here
      </body>
    </html>

Elements can be selected inside the ``<style>`` element using curly braces ({ }):

    <style>
      element {
        property: value;
      }
    </style>

Using it with class ``.`` and id ``#``:

    <!DOCTYPE html>
    <html>
      <head>
        <style>
          span {
            text-decoration: underline;
          }

          #red-word {
            color: red;
          }

          #blue-word {
            color: blue;
          }
        </style>
      </head>
      <body>
        <p>
          Roses are <span id="red-word">red</span>.<br />
          Violets are <span id="blue-word">blue</span>.<br />
        </p>
      </body>
    </html>

## Google Forms

In HTML:

    <form action="" method="">
      <!-- More code will go here -->
    </form>

Two attributes are commonly used with the ``<form>`` element:

- The ``action`` attribute that says where the form data should go after it is submitted.
- The ``method`` attribute for how the form data is processed.

## Inputs

The ``<input>`` element as an interactive control for entering data. A type attribute is used to determine the kind of input to use. While there are many types of inputs, the two we'll use most often are:

A text value that renders a plain textbox on the form.

    <form>
      <input type="text">
    </form>

A submit value that turns the ``<input>`` element into a button for submitting the form data.

    <form>
      <input type="submit">
    </form>

Note: The ``<input>`` element uses a self-closing tag.

Example:
<form>
  <input type="text">
  <input type="submit">
</form>

## Sign Up

### Input Type: Emails

``<input type="email">``

This tells the form to expect a text input with the typical email syntax (including the @ symbol).

### Input Type: Passwords

``<input type="password">``

Dots will replace the text that would otherwise appear in the text box:

### Input Validation

Forms can also mask text input if the ``<input>`` element has a "password" type. We can even give it a ``minlength`` and ``maxlength`` attribute to further validate the input:

    <input type="password" minlength="4" maxlength="10">

### Required Data

The ``required`` attribute can be applied to one or more form inputs to enforce this.

    <form method="dialog">
      Name: <input type="text" required>
      <br><br>
      Favorite Color: <input type="text">
      <input type="submit">
    </form>

### Input Type: Number

To prompt the ``<input>`` element for numbers, we do the following:

    <input type="number">

Example:
<input type="number">

#### ``step`` Attribute

    <input type="number" step="2">

<input type="number" step="2">

Makes the value for going up or down a number by 2.

A max and min attribute can be used to set how high or low this input can go:

    <input type="number" min="1" max="42">

Input Type: Checkbox and Radio

``"checkbox"`` type renders as a box that is ticked off to mark the input as "finished" or "complete."

    <h3>Favorite Movie Genres</h3>
    <input type="checkbox"> Action<br>
    <input type="checkbox"> Sci-Fi<br>
    <input type="checkbox"> Rom-Com<br>
    <input type="checkbox"> K-Drama<br>
    <input type="checkbox"> Documentary<br>

Radio buttons are lists of options.

    <h3>Which do you think?</h3>
    <input type="radio"> Yanny
    <br>
    <input type="radio"> Laurel

### Textareas

The ``<textarea>`` element renders as a plain, mini-text editor on the web page.

    <textarea id="data-entry" rows="7" cols="42"  placeholder="Enter some data here!"></textarea>

<textarea id="data-entry" rows="7" cols="42"  placeholder="Enter some data here!"></textarea>

In addition to class and id, the ``<textarea>`` uses the following attributes:

``rows``: The amount of visible rows, or text lines (defaulting at 2).

``cols``: The number of visible columns in average character widths (defaulting at 20).

``placeholder``: Some default text meant to explain what kind of data should be entered.

The required attribute can be applied to the 
``<textarea>`` element, too.

### Form Labels

Labels can be used in forms to associate pieces of text with form controls and inputs.

    <form>
      <label>Book Title: </label><input type="text">
      <br><br>
      <label>Author: </label><input type="text">
      <br><br>
      <input type="submit">
    </form>

    <form>

    <!-- 
    
    Simply defined as: 
    
    <form>
      <label>Book Title: <input type="text"></label>
      <label>Author: <input type="text"></label>
    </form>
    -->

<label>Book Title: </label><input type="text">
<br><br>
<label>Author: </label><input type="text">
<br><br>
<input type="submit">
</form>

## The Header

The ``<header>`` element always goes in the ``<body>`` element. It usually contains a heading element ``(<h1>-<h6>)``.

    <body>
      <header>
        <h1>Welcome to My Site!</h1>
      </header>
    </body>

*Note: This is not to be confused with the ``<head>`` element that exists outside the ``<body>`` element.*

## Navigation

The semantic element used for this is the ``<nav>`` element. This usually goes inside of a ``<header>`` element.

    <header>
      <nav>
        <!-- Links go here. -->
      </nav>
    </header>

The ``<nav>`` element may contain ordered lists, unordered lists, or a combination of both.

## Main & Footer

### Main

Where all the main information goes; uses  ``<main>``.

    <body>
      <main>
        <!-- Main information goes here. -->
      </main>
    </body>

### Footer

The information in this element usually goes beneath the main content of the page, uses ``<footer>`` and it includes:

- The name of the company/creator(s) of the page.
- Some copyright information.
- Additional navigation links to other sections or other sites.


        <footer>
        <!-- Footer content goes here. -->
        </footer>

## Page Sections

We use the ``<section>`` element to group pieces of related content together.

    <main>
      <section>
        <h2>Section A</h2>
      </section>
      <section>
        <h2>Section B</h2>
      </section>
      <section>
        <h2>Section C</h2>
      </section>
    </main>

*Note: Unlike the ``<main>`` element, a page can have multiple ``<section>`` elements!*

## Single Articles

While the ``<section>`` element groups together pieces of related content, **we use the ``<article>`` element for those singular pieces of content.**

    <section>
      <h2>Section Heading</h2>
      <article>
        <h3>Article Heading</h3>
        Piece of content
      </article>
    </section>

While not required, an ``<article>`` element should begin with a heading element (much like with a ``<section>`` element).

You can also nest an ``<article>`` within another ``<article>`` element. This is usually done if there is a piece of standalone markup within a single piece of content (e.g., a single comment from a single blog post).

## Figures

A "figure" is usually a graphic, image, or diagram.

    <figure>
      <!-- Figure content goes here. -->
    </figure>

While the contents in a ``<figure> ``element are grouped together, they can be placed either in the page's main content or somewhere else.

## Captioning Figures

The ``<figcaption>`` element is used to describe what is in the ``<figure>`` element.

    <figure>
      <img
        width="500"
        src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a5/Tsunami_by_hokusai_19th_century.jpg/1024px-Tsunami_by_hokusai_19th_century.jpg"
        alt="Great Wave off Kanagawa by Hokusai"
      />
      <figcaption>The Great Wave Off Kanagawa by Hokusai</figcaption>
    </figure>

<figure>
  <img
    width="500"
    src="https://upload.wikimedia.org/wikipedia/commons/thumb/a/a5/Tsunami_by_hokusai_19th_century.jpg/1024px-Tsunami_by_hokusai_19th_century.jpg"
    alt="Great Wave off Kanagawa by Hokusai"
  />
  <figcaption>The Great Wave Off Kanagawa by Hokusai</figcaption>
</figure>

We can also use the ``<figcaption>`` element to describe multiple pieces of content within the ``<figure>`` element:

    <figure style="margin:0;display:inline;">
      <img
        width="150"
        src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/00/Brooklyn_Bridge_Manhattan.jpg/250px-Brooklyn_Bridge_Manhattan.jpg"
        alt="Brooklyn Bridge"
      />
      <img
        width="150"
        src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/3a/Prospect_Park_New_York_October_2015_003.jpg/1024px-Prospect_Park_New_York_October_2015_003.jpg"
        alt="Prosepct Park, Brooklyn, NY, USA"
      />
      <img width="150"
      src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f0/Coney_Island_beach_and_amusement_parks_%28June_2016%29.jpg/1024px-Coney_Island_beach_and_amusement_parks_%28June_2016%29.jpg"
      alt="Coney Island, Brooklyn, NY, USA" />

      <figcaption>Notable Brooklyn spots (from left to right): Brooklyn Bridge; Prospect Park; Coney Island</figcaption>
    </figure>

<figure style="margin:0;display:inline;">
  <img
    width="150"
    src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/00/Brooklyn_Bridge_Manhattan.jpg/250px-Brooklyn_Bridge_Manhattan.jpg"
    alt="Brooklyn Bridge"
  />
  <img
    width="150"
    src="https://upload.wikimedia.org/wikipedia/commons/thumb/3/3a/Prospect_Park_New_York_October_2015_003.jpg/1024px-Prospect_Park_New_York_October_2015_003.jpg"
    alt="Prosepct Park, Brooklyn, NY, USA"
  />
  <img width="150"
  src="https://upload.wikimedia.org/wikipedia/commons/thumb/f/f0/Coney_Island_beach_and_amusement_parks_%28June_2016%29.jpg/1024px-Coney_Island_beach_and_amusement_parks_%28June_2016%29.jpg"
  alt="Coney Island, Brooklyn, NY, USA" />

  <figcaption>Notable Brooklyn spots (from left to right): Brooklyn Bridge; Prospect Park; Coney Island</figcaption>
</figure>