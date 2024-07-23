# Assignment: Use WAI-Aria when necessary

The input field in the `input.html` file in this directory has additionally to it's label a hint (below the input field) that provides the user with instructions how to provide correct input.

While the hint and the input are visually clearly connected they are not in a programmatic way: when users navigate via keyboard to the input field the screen reader will read the label of the input field out, tell the user that they are currently on an input field where they can enter text and then stop without reading the additional hint. 

You can try it yourself by opening the `input.html` in a browser and activating your screen reader of choice.

## Your turn

How could you use WAI-Aria to programmatically connect the input hint with the actual input? Add the respective code to the `input.html` file.
