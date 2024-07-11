# The Origins of HTML

 All my notes, resources, and the activities I made to learn HTML from Codédex

## Elements

An ``element`` usually consists of an opening tag, the content, and a closing tag. A tag is enclosed in angle brackets.

    <p>Hello World!</p>

The ``<p>`` paragraph element tells the browser that the content inside is "paragraph" text.

The ``<body>`` element defines an HTML document's "body" and it's where any content that we want to display to the user will be held:

    <body> opening tag begins the "body".
    <p>👋 I'm a new web developer!</p> is some text in a paragraph element.
    </body> closing tag ends the "body".

***There can only be one ``<body>`` element in an HTML file.***

## Heading

Suppose we want to add a headline to our website that displays a news article. Here's how we would do it using a ``<h1>`` heading element and a ``<p>`` paragraph element.

There are six levels of section headings, from ``<h1>`` to ``<h6>``

***Note: Only one ``<h1>`` element should be used in a .html file.***

## Line Break

Pressing enter won't do us any good because HTML ignores multiple spaces and line breaks within elements.

Line break is ``<br>``

A self-closing tag doesn't need to be closed manually by a closing tag (i.e., it does not have a separate closing ``</tag>``). The break tag is the first one we have encountered.

## Text Formatting

- ``<b>`` element to bold text.
- ``<i>`` element to italicize text.
- ``<u>`` element to underline text.
- ``<s>`` element to strikethrough text.

        <b>This text is using bold formatting.</b><br>
        <i>This text is using italics formatting.</i><br>
        <u>This text is using underline formatting.</u><br>
        <s>This text is using strikethrough formatting.</s><br>

***Note: The ``<b>`` element is just for bolding text stylistically; HTML also has a ``<strong>`` element used to convey that the content inside is important, as well as styling it to be bold.***