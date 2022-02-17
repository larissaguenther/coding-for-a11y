# Accessible Images

## Check 1: Images that have only decorative purpose and don't contain any relevant content are hidden for screen readers

Images that are non-functional and non-meaningful should be hidden from the screen reader, so it doesn't read the image out.

You can do this by setting the image purely in CSS as a background image:

```
body {
    background-image: url("image.png");
}
```

or you use the `aria-hidden` attribute within the image HTML element:

```
<img aria-hidden="true">
```

## Check 2: All images that are relevant for the purpose of a page provide a programmatically connected description of the image

When an `<img>` tag does not contain an `alt` attribute screen readers will read the `src` attribute of the image instead, which is not very helpful

Always use the `alt` attribute within an `<img>` tag and provide a well-written description of the image. 

```
<img alt="description of image">
```

Tip: Screen readers will announce `<img>` tags by reading out "Image". So don't use wordings like "Image of..." or similar in your `alt` description as this would just be a repition of what the screen reader will say anyways. 

If your image already has a visually connected description, for example with a `<figcaption>` tag, you can connect this description also programmatically to the image, so the screen reader reads it for for the image by using `aria-labelledby`. 

```
<figure>
    <img alt="" aria-labelledby="caption">
    <figcaption id="caption">Description of image</figcaption>
</figure>
```

It is important here to provide an empty `alt` attribute so the image is accessible. When the `alt` attribute is empty the screen reader will just skip it and read out the figcaption instead, which is connected with the image via the `aria-labelledby` attribute.