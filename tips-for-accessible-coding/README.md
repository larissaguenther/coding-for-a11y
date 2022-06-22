# Tips for accessible coding

While coding these 5 rules can help you code in an accessible way:

## 1. Use semantic HTML

- use native semantic HTML elements whenever possible
- use semantic HTML elements for the correct purpose: e.g. list tags (`<ul>`, `<ol>`, `<li>`) only for lists, `<table>` tags only for tabular data and not for layout purpose, `<img>` tag for images etc.
- use native HTML elements in the correct intended way: e.g. provide an associated `<label>` tag for all `<input>` elements 

## 2. Write well-structured HTML

- use only one `<h1>` tag per page
- order heading tags `<h1>`, `<h2>`, etc. hierarchically 
- make sure the HTML content is in a logical order so it still makes sense without CSS styling
- group related content in logical sections, e.g. using `<header>`, `<main>`, `<footer>`, `<section>`, etc.

## 3. Support Keyboard Navigation

- make sure all interactive elements are focusable and reachable by keyboard in a logical order, don't mess with the `tabindex`
- make sure all focusable elements have an outline, never remove the `outline` property
- apply JavaScript event handlers only to interactive elements that can receive keyboards focus (not `<div>`)

## 4. Hide non-functional and non-meaningful non-text content from assistive technologies 

- include background images via CSS (`background-image`)
- hide other non-functional images, icons etc. via `aria-hidden="true"`

## 5. Provide descriptions for all functional and meaningful non-text content

- use an `alt` attribute or `aria-label` to describe images or other non-text content 
