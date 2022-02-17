# Use WAI-Aria when necessary

## What is WAI-Aria?

WAI-Aria stands for Web Accessibility Initiative - Accessible Rich Internet Applications.

It provides a set of additional HTML attributes that can be applied to elements to provide additional semantics and improve accessibility wherever it is lacking. There are basically three different kinds of attributes:

### Aria roles

Aria roles define what an element is and what it does, e.g. `role = "button"`. The element will be announced by that role by the screen reader.
Semantic elements already have a role by default, so you don't have to provide it. But you can use aria roles to describe non-semantic elements that don't have a role by default.

### Aria properties

Aria properties provide an element with extra meaning or semantics that are not provided by default. 

### Aria states

Aria states are properties that change throughout the lifecycle of an app, generally programmatically via JavaScript.You can use it to define the current conditions of an element.

## Useful resources

- [Aria roles](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Roles)
- [Aria states and properties](https://developer.mozilla.org/en-US/docs/Web/Accessibility/ARIA/Attributes)