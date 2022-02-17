# Support Keyboard Navigation when not supported by default

When you are using native HTML elements keyboard navigation should usually be supported and accessible by default. There are a few things you should pay attention to, to make sure keyboard navigation is properly supported:

## Outline property

The outline is a line that is drawn around elements to make the elements stand out when focused - it should be used to show keyboard users which element they are currently focusing. Most interactive elements have an outline by default. You should **never remove the outline property** by setting `outline: none` in your stylesheet.

Always check if all elements that are focusable by tab have an outline, add an outline if necessary.

## Tabindex attribute

The tabindex indicates if an element can be focused and where it participates in sequential keyboard navigation. All native interactive HTML elements have a tabindex by default and the tabindex order is defined by the documents source order. 
- `tabindex="-1"` removes the element from sequential keyboard navigation (but it is still clickable!)
- `tabindex="0"` adds the element to the sequential keyboard navigation
- `tabindex = "1"` or any positive value defines the order of keyboard navigation, **never do this!**

## Event Handlers

Apply JavaScript event handlers (`onclick` etc.) only to interactive elements that can receive keyboard focus.  
For example you can apply it to a `<button>`, but not to a `<div>`.

## Useful Resources

- [Outline property](https://developer.mozilla.org/en-US/docs/Web/CSS/outline)
- [How to use the tabindex attribute](https://www.a11yproject.com/posts/how-to-use-the-tabindex-attribute/#:~:text=tabindex%20is%20a%20global%20attribute,via%20the%20keyboard's%20Tab%20key.)