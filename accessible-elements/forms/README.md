# Accessible Forms

## Check 1: All inputs have a clearly described and associated label

Provide labels to identify all form controls. Labels need to clearly describe the purpose of the form control.

### Best case: `<label>` element is used

Whenever possible use the `<label>` element to associate text with form elements explicitly.

The `for` attribute of the label must exactly match the `id` of the form control.

```
<label for="name">Name</label>
<input type="text" name="name" id="name">
```

Label should usually come before the input field within the HTML structure. Labels for radio buttons and checkboxes are also accessible when they come after the input.

```
<input type="checkbox" name="agree" id="agree">
<label for="agree>I agree with the terms and conditions</label>
```

### Fallback: `aria-label` or `aria-labelledby` is used

If for some reason you are not able to use the `<label>` element you can use the WAI-Aria attributes `aria-label` or `aria-labelledby`.

Both attributes are not visually displayed in the browser, so they should only be used when the label of the input is visually clear from the surrounding content on the website.

```
<input type="text" name="search" aria-label="Search">
<button type="submit">Search</button>
```

```
<input type="text" name="search" aria-labelledby="searchbutton">
<button id="searchbutton" type="submit">Search</button>
```

## Check 2: 