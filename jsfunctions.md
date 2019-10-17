# Notes on Duckett: Scripts, Expressions/Operators, Functions

## What is a script and how to write one?
pgs. 1-24

#### A script is a series of instructions
- Script: a series of instructions a computer can follow to achieve a goal. 
#### Writing a script
- To write a script, know the goal of the script and list the tasks needed to be completed. 
  - Define the goal
  - Design the script
  - Code each step

#### Designing a script
- Tasks: design a flowchart to see how tasks flow down to one another and take paths depenending on user inputs. 
- Steps: Each task can be broken down into steps. 

#### From steps into code
- Know vocabulary and syntax to translate human language into code. Understand how to think like a computer by taking a _programmatic_ approach to problem-solving. 

#### Defining a goal and designing the script
- Detail your goals for the script. 
- Break goals down into tasks

#### Sketching out tasks in a flowchart
- Use flowcharts to show the paths between each step. 


## Expressions and operators
pgs. 74-79
#### Expressions
- Expression: evaluates into a single value. 
- Types of expressions:
  - Those that assign a value to a variable
    - `var color = 'beige';`
  - Those that use 2+ values to return a single value
    - `var area = 3 * 2;`

#### Operators
- Expressions rely on operators to create a single value from 2+ values. 
- Types of operators:
  - Assignment operators `=`
  - Arithmetic operators `+ - / * // -- %`
  - String operators (concatenation via `+`)
  - Comparison operators (`>` `<`)
  - Logical operators (`&&` `||` `&`)

#### String operator
- When quotes are placed around a number, it is a string. Cannot perform addition operations on strings. 
- If you try to add numeric data type to a string, number becomes part of the string. String takes precedence. 
  - If any other arithmetic operators used on a number and a string, value will result in a `NaN` (not a number). 

## Functions
pgs. 88-94

#### What is a function?
- Functions group series of statements together to perform a specific task. If different parts of a script repeat this task, you can call this function as needed. 
- Functions sometimes need to be provided with information, or _parameters_, in order to do their work. 
- When a function is expected to provide an answer, the response is a _return value_. 
- Functions can be anonymous; they are not given a name. The upside is less code is written to declare this function compared to other functions, only if the function is immediately used. The downside is that the function cannot be used again. 

#### Declaring a function
- ```
  function sayHello() {
  document.write(document.write('Hello!')};
  ```
- Functions are declared with the _function keyword_ `function`. 
- A function is given a name, followed by parentheses `sayHello()`. 
- The statements that perform the task sit in a code block, which are surrounded by curly braces `{document.write('Hello!');}`

#### Calling a function
- Once function is declared, you can execute all the statements between the curly braces with just one line of code. 

#### Declaring functions that need information
- Fill in _parameters_ within the parentheses of the function. 

#### Calling functions that need information
- When a function with parameters is called, you specify the values it needs. These values are called _arguments_. Arguments can be pre-fixed values or variables. 
