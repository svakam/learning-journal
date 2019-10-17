# Duckett: Operators and Loops

pgs. 150-151, 156, 157, 170-173, 176

## Operators
pgs. 150-151, 156, 157

#### Comparison operators: evaluating conditions
- Evaluate a situation by comparing 1 value in script to what is expected. Result will be a Boolean (true or false). 
  - `==`: is equal to
    - Compares two _values_ to see if they're the same. 
  - `!=`: is not equal to
    - Compares values to see if they're not the same. 
  - `===`: strict equal to
    - Compares to see if both data type _and_ value are the same. 
  - `!==`: strict not equal to
    - Compares to see if both data type and value are not the same
  - `>` and `<`: greater than, less than
    - checks if number on left is greater than or less than number on right. 
  - `>=`:  greater than or equal to
  - `<=`: less than or equal to

#### Logical operators
- Return single values of true or false.
- Allow comparing results of more than 1 comparison operator. 
- ((5 < 2) && (2 >= 3))
- `&&`: logical and
  - Tests _more than_ one condition. 
  - If both expressions evaluate to true, then expression returns true. 
  - If just one expression is false, whole expression returns false. 
- `||`: logical or
  - Tests _at least_ one condition. 
  - If either expression is true, whole expression returns true. 
  - If both are false, whole expression returns false. 
- `!`: logical not
  - Takes in single Boolean value and inverts it. 
  - !true returns false. 
  - !false returns true. 

## Loops
pgs. 170-173, 176

#### Loops intro
1. Loops check a condition. 
2. If it returns true, code block runs. 
3. Condition checked again. 
4. Repeat 1-3 until false. 
5. If condition is false, exits the loop and resumes down your code. 

- For loops: if code needs to be run a specific number of times, a variable will be initialized as a counter, condition is checked, code is executed, and then counter is incremented. Repeat this process until condition is false. 
  - `for (var i = 0; i < 10; i++) { //code }`
  - Initialization: `var i = 0;`
  - Condition: `i < 10;`
  - Update: `i++;`
    - Same as `i = i + 1;` `i += 1;`. 

- While loops: if it is unknown how many times a loop should run, code will run until condition is not met. 
  - `while (//condition) {code}`

- Do while loops: code runs _at least_ once, then checks condition to see if code should run again. 
  - `do {code} while (//condition)`


