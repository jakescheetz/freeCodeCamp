# CSS Notes
> Jacob Scheetz, 2022

### Inline Styling 
- this can be done by putting a style attribute on the element you want to style, for example: 
```
<h2 style="color: blue;">
```
- see 'change-the-color-of-text.txt'

### Style blocks in HTML
- you can use style tags to insert CSS directly to a page 
- good use if you want to style multiple of the same elements: 
```
<style>*CSS Here*</style>
```
- see 'use-css-selector-to-style-elements.txt'

### CSS classes
- good for reusing styling
- add the class attribute to an element to match the defined CSS class to apply it's styling
- CSS defintions need to start with a period
- see 'use-a-css-class-to-style-elements.txt'

### Font
- size is controlled by font-size property: 
```
h1 {
  font-size: 30px;
}
```
see: 'change-the-font-size-of-an-element.txt'
- font can be changed with font-family
- you can pull in third party fonts like from google: 
https://fonts.googleapis.com
- this can be done by using a link element and then specifying the family name in CSS definitions: 
```
<link href="https://fonts.googleapis.com/css?family=Lobster" rel="stylesheet" type="text/css">
... 
font-family: FAMILY_NAME, GENERIC_NAME;
```
- see: 'import-a-google-font.txt'

### Borders
- can be controlled by several properties (see the example file for this topic)
- important to note multiple classes can be applied to a singular element as long as they are separated by spaces
- see 'add-borders-around-your-elements.txt'
- to round the edges on borders, use the border-radius field
  - this can be used on images and borders alike!
- you can use percentages on the border-radius property to make an image circular

### Element id's
- id's should be unique for each element
- they are another method of providing unique styling similar to classes
- instead of .name, we use #name when specifying a styling for an id
- see 'use-an-id-attribute-to-style-an-element.txt'