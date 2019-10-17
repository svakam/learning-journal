# Notes on Duckett: JS & Query, Pages 43-69

How do you write a script for a web page?

#### How HTML, CSS and JS fit together
- HTML = content layer; added first.
- CSS = enhances HTML with rules that state how content is presented; added next in a separate file.
- JS = changes how page behaves by adding interactivity; added last in a separate file.

#### Creating a basic JS
- Written in plain text like HTML/CSS, so don't need any new tools to write a script.
- Use HTML's `<script>` to tell browser it's coming across a script.
  - `<script>`'s `src` attribute tells where JS located.

#### Source code is not amended
- If separate JS file used, HTML remains the same, despite JS using HTML elements for its functionality.
- Only the link to the JS file would be added.

#### Placing script in page
- It's preferred not to mix JS in HTML.

#### Objects and methods
- `document.write('Good afternoon!')`
  - `document` = object
    - Objects contain several methods and properties, the latter of which can be _called_.
  - `.` = member operator
    - Members of the object can be accessed via this operator. 
  - `write('Good afternoon!')` = method
    - A method accomplishes something desired to be done (ex. writing new content into the page). 
  - `'Good afternoon!'` = parameter
    - Methods require some info input in orer to work, and this data goes into the parameter portion (ex. write needs an input of what to write). 

#### JS runs where it is found in the HTML
- When JS is encountered via `<script>`, browser stops to load the script and does what is needed within the tags. 

#### Statements
- Script: a series of instructions a computer can follow. 
- Statement: each individual instruction/step. 
  - Must end with semicolon `;`. 
  - Each one starts with a new line. 
  - Can be organized into code blocks. 

#### Comments
- Explains what the code means to a code reader/reviewer. 
  - `//` preface to a single-line comment. 
  - `/* */` multi-line comments included within this. 

#### Variables
- Scripts need to store temporary information to do its job, and this information is stored in variables. 
- Variables are declared with `var`, followed by the variable name, followed by a `;`. 
  - `var quantity;`
- Can assign values to variables with _assignment operator_ `=`. 
  - `quantity = 3;`
- Shorthand for creating variables:
  - `var a, b, c; a = 5; b = 14; c = a * b;`
  - `var a = 5, b = 14; var c = a * b;`
- Can change variable values downstream in your code as needed. 

#### Data types
- Numeric: `0.75`
- String: `'Hello'`
- Boolean: `true`, `false`

#### Using variables to store a number, string or boolean
- Can assign a number to a variable, and assign a variable to a variable, the former of which can be dependent on what that first number was. 
- Strings are placed within single or double quotes. 
- Sometimes quote marks need to be used within a string. Because strings can live in single/double quotes, the inner string can be double-quoted, and the main string can be single-quoted, or vice versa. Can also _escape_ quotation characters by a backwards slash `\`. 
  - `message = '<a href=\"sale.html\">25% off!</a>';`
- Booleans are used when the value can only be true or false AKA on or off AKA 1 or 0. Used for code that takes multiple paths, and one path is desired depending on the variables used. 