# Use semantic, well-structured HTMl when possible

## What is semantic HTML?

Semantic HTML elements clearly describe their meaning and the content they are supposed to contain to developers and the browser.  
Especially screen readers rely on native HTML semantics.

Semantic elements are for example `<table>`, `<form>` or `<section>` - they all have a clearly defined content.

Non-semantic elements are for example `<div>` and `<span>` - they tell nothing about their content.

## What is well structured HTML?

An unstyled view of an HTML document approximates the way it would be read by a screen reader. You should check how your page looks like when disabling the styles: the structure should still be clear and easy to understand without styles. 

Therefore you should use semantic HTML elements in a logical and hierarchical way, for example use only one `<h1>` tag per page, and separate your content in logical sections, e.g. use the `<header>` tag for introductory content at the top of your page.

## Useful Resources

- [HTML Semantics Cheat Sheet](https://learn-the-web.algonquindesign.ca/topics/html-semantics-cheat-sheet/)
- [HTML Semantic Elements](https://www.w3schools.com/html/html5_semantic_elements.asp)