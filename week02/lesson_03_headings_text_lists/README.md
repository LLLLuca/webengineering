# Table of Contents
- [HTML elements for headings, text and lists](#html-elements-for-headings--text-and-lists)
  * [Headings](#headings)
  * [Text](#text)
  * [Unordered and Ordered Lists](#unordered-and-ordered-lists)
- [Links](#links)

# HTML elements for headings, text and lists

The following explanations reference the source file [`01_headings_text_lists.html`](https://github.com/winf-hsos/webengineering/blob/master/week02/lesson_03_headings_text_lists/01_headings_text_lists.html).

```html
<!DOCTYPE html>
<html>

<head>
    <meta charset="utf-8">
    <title>Haster Bier Online-Shop</title>
    
     <style>
        /* Set the standard font for the document */
        body { font-family: 'Open Sans'; }
        
        h1, h2 {
            color: #009EE3; /* Make all <h1> and <h2> HS-blue */
        }
    </style>
</head>

<body>
    <!-- Top-Level Heading -->
    <h1>Willkommen in unserem Online-Shop</h1>
    
    <!-- Level 2 Heading-->
    <h2>Hell order Dunkel?</h2>
    
    <!-- A paragraph of text -->
    <p>Bestellen Sie unsere Haster Biere bequem online:</p>
    
    <!-- An unordered list -->
    <ul>
        <li>Haster Helles</li>
        <li>Haster Dunkles</li>
    </ul>
    
    <h2>Kontakt</h2>
    <!-- An ordered list -->
    <ol>
        <li>Anke Riemenschneider - 0541 969 5269</li>
        <li>Dorothee Frickhofen -  051 969 5346</li>
    </ol>
    
</body>

</html>
```

## Headings

Headings help structure your text and website, similar to how you  structure a word document: The title of a chapter could be the highest level, and for subsections you can use lower level headings. This approach is also used in websites, for which HTML povides six different headings:

```html
<h1>Top Level Heading</h1>
<h2>Level 2 Heading</h2>
<h3>Level 3 Heading</h3>
<h4>Level 4 Heading</h4>
<h5>Level 5 Heading</h5>
<h6>Level 6 Heading</h6>
```

Per default, each of the headings has a certain standard appearance in a browser: The higher the level, the smaller the font size. However, we can modify this appearance using CSS, so to change the font size of a level 2 heading, we could write this CSS rule:

```css
h2 {
    font-size: 18px;
}

```

That's a bit smaller than the default size. (Look up the default CSS property values for headings [here](https://www.w3schools.com/tags/tag_hn.asp)).

Besides structuring the text visually for the ready through appearance, there is another important reason to use the HTML headings: Search engines such as Google use theses tags to index the website. So if Google encounters a heading, it'll assume that the text below it is associated with the words in the heading. This in term will make the website easier to find in a Google search. When your are not using HTML headings at all (for visual structure, you could format a paragraph or `<span>` element to look like a heading), Google has no way of knowing the structure and important keywords of your website, leading to bad SEO and less traffic.

## Text

Text is probably the most important content on any website. While you can put text anywhere in your document, the preferred HTML tag for plain text is the `<p>` tag, which is short for a paragraph.

```html
<p>Bestellen Sie unsere Haster Biere bequem online:</p>
```

A HTML paragraph per default is a so called *block element*, meaning it will be displayed in its own line. So if you have two `<p>` elements in one line in your source code, the result will be two lines with a small space inbetween.

```html
<p>Kostenlose Lieferung!</p><p>Wir freuen uns auf Sie!</p>
```

As with any HTML element, you can apply CSS styles to change the default appearance.

## Unordered and Ordered Lists

To create a bullet point list, which is unordered, simply use the `<ul>` tag. For ordered and therefore numbered lists, use the `<ol>` tag. To create an item within a list, use the `<li>` tag. The example below illustrates that.

```html
<!-- An unordered list -->
<ul>
    <li>Haster Helles</li>
    <li>Haster Dunkles</li>
</ul>

<!-- An ordered list -->
<ol>
    <li>Sign up for our shop</li>
    <li>Place your order</li>
</ol>
```

# Links

- [HTML Headings at W3Schools.com](https://www.w3schools.com/html/html_headings.asp)
- [HTML Paragraphs at W3Schools.com](https://www.w3schools.com/html/html_paragraphs.asp)
- [HTML Lists at W3Schools.com](https://www.w3schools.com/html/html_lists.asp)