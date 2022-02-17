# Accessible HTML Elements Checklist

## Headings

Use headings to create a well structured and meaningful content outline.

### h1 headings
Use only **one singular** `<h1>` heading per page to title or describe the main function of the page

### h2 headings

Use `<h2>` headings to describe second-level headings

### h3 to h6 headings

Use `<h3>`, `<h4>`, `<h5>` and `<h6>` in a descending hierarchial order to break content down even further.

### Checklist

- Only one `<h1>` element is used per page
- All heading tags are used in descending hierarchical order - same semantic hierarchy means same heading tag 

## Inputs

### Validating input

- use the `required` attribute for required inputs to programatically indicate that they are required
- use HTML input types to validate data: `email`, `url`, `number`, `range`, `date` or `time`
- input types often provide additional parameters to help to limit and validate input, e.g. `maxlength`, `min`, `max` or `steps`
- use the `pattern` attribute to use regular expressions to specify custom formats for the input