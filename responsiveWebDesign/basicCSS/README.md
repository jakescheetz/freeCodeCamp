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

### Padding / Margins 
- all HTML elements are essentially rectangles
- the padding controls the amount of space that the item will take up in the overall structure (vertical spacing)
- the margin controls the space between the border and the padding (horizontal spacing)
- margins can be negative to make a smaller element take up a whole element
- margin/padding have a top, right, bottom, left control
- instead of individually specifying the size of each side on an element, use clockwise notation: 
  - top, right, bottom, left
  - ``` padding: 10px 20px 10px 20px; ```
  - this works with margin too
  - see 'use-clockwise-notation-to-specify-elements.txt'
- sizing can be relative (em instead of pixels)
  - this is based off of the font-size

### Other selectors
- you can use the notation: 
``` [type='checkbox']{ styling here} ```
to selector an element of a specific type to style something
- see 'use-attribute-selectors-to-style-an-element.txt'

### CSS Inheritence
- every html file automatically inherts a body element 
- if you style something specifically with a selector than that takes precedence over inheritence
- if an element has multiple classes of styles the class that was defined last in the style sheet will take predence over the others
- id styling has even higher precedence than classes
- inline styling has the highest precedence
- the syntax ```!important``` can be added to any CSS element to give it the highest order of precedence

### CSS colors
- can also use hex instead of the keyword system 
- hex uses six digits to specify a color 
  - a 0 represents the absence of color
  - see 'use-hex-code-to-mix-colors.txt'
- you can use three digits instead of six but it makes customization less workable
- can also use the rgb notation: 
``` rgb(0-256, 0-256, 0-256) ```

### CSS Variables
