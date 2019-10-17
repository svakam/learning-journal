# Notes on Duckett: CSS Intro

## Chapter 10: Introducing CSS

**CSS:** Allows creation of rules that specify how content of an element should appear. 

Once you know how to write a CSS _rule_, learning CSS just involves knowing the various properties you can use to make your website appear more appealing. 

#### Understanding CSS: Thinking inside the box
- It can be said there is an 'invisible box' around every HTML element. Each element can be treated differently or the same as others when using CSS. Recall block-level and inline elements. 

#### CSS associates style rules with HTML elements
- `p {font-family: Arial;}`
  - CSS rule contains 2 parts:
    - A _selector_ and
    - a _declaration_. 
    - Selectors indicate which element the rule applies to. The same rule can apply to more than one element if you separate element names with commas. 
    - Declarations indicate how the elements referred to in the selector should be styled. Declarations sit inside curly brackets. 
      - Declarations are made of a _property_ and a _value_ in that order, separated by a colon. 
        - Properties indicate the **aspects** of the element you want to change (color, font, width, height, border). 
        - Values are the specific settings desired for the properties (e.g. yellow, Arial, 360, 240, etc.)
  - In this example, _p is the selector_, and _font-family: Arial_ is the declaration. 
    - This indicates all `<p>` elements should be shown with Arial typeface. 
- `h1, h2, h3 {font-family: Arial; color: yellow;}`

#### Using external CSS
- `<link>`
  - Used in .html file to tell browser where to find the CSS file. It is an _empty element_ (does not need a closing tag). 
  - Lives inside `<head>`. 
  - It should use 3 attributes:
    - `<href>`
      - Specifies path to CSS file, which is often placed in folder called `css/` or `styles/`. 
    - `<type>`
      - Specifies type of doc being linked to, whose value should be `text/css`. 
    - `<rel>`
      - Specifies relationship between HTML and file it's linked to; value should be `stylesheet` because that's what the CSS is in relation to HTML. 
  - More than one CSS stylesheet can be used for an HTML page (ex. one CSS can control presentation, another can control layout). 
- `<link href="css/styles.css" type = "text/css" rel="stylesheet" />`

#### Using internal CSS
- `<style>`
  - Can include CSS rules within HTML by placing them inside this element. 
  - This also sits inside `<head>`. 
  - Uses `type` attribute to indicate styles are specified in CSS; value should be `text/css`. 
  - When building a site with more than 1 page, an external style sheet is preferred. Allows all pages to use the same style rules, keeps content separate from appearance, and can make quicker changes based on the one file rather than arduiously going through the HTML and looking for the places to change in each page. 
- `<style type="text/css">`


#### CSS selectors
- _Selectors_ allow targeting of rules to specific documents in HTML. 
- Case sensitive! 
- Examples:
  - Universal selector `* {}`
    - Applies to all elements in document
  - Type selector `h1, h2, h3 {}`
    - Matches element names
  - Class selector `.note p{}`
    - Matches element whose `class` attribute has value that matches the one specified after the `.` symbol
    - `p.note {}`
      - Targets only `<p>` whose `class` has a value of `note`
  - ID selector `#introduction {}`
    - Matches element whose `id` has value that matches the one after the `#` 
  - ...and much more

#### How CSS rules cascade
If 2+ rules apply to the same element:
- Last rule
  - If 2+ selectors are identical, the latter of the two take precedence
- Specificity
  - If 1 selector is more specific than the others, the more specific rule will take precedence over more general ones
- Important
  - Add `!important` after any property value to override precedence rules

#### Inheritance
- If a declaration (ex. font-family, color) is applied to an HTML element (ex. `<body>`), the declaration will apply to most child elements, and the declaration's value (ex. Verdana) will be _inherited_ by the children. 
- Properties may be _forced_ to inherit values from parent elements by using `inherit` for the value of the peroperties (ex. `padding: inherit;`) 

## Chapter 11: Color

How do we specify colors? What is color terminology? How to use contrast? How to apply background colors? 

#### Foreground color
- **RGB values:** `rgb(<number 0-255>, <number 0-255>, <number 0-255>)`
- **Hex codes:** 6-digit codes preceded by a pound sign `#xxxxxx`
- **Color names:** CSS has pre-defined color names recognized by browsers

#### Background color
- `background-color: <RGB value>` or `<hex>` or `<color name>`

#### Understanding color

#### Contrast

#### Opacity

#### HSL Colors

#### HSL & HSLA