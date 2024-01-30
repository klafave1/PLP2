## PLP2 (Swift)

### 1. What are the naming requirements for variables in your language? a. What about naming conventions? Are they enforced by the compiler/interpreter, or are they just standards in the community?

##### Naming Requirements:
* Variables must start with either a letter or an underscore, which can then be followed by other letters, underscores, and digits. 
* Swift is case-sensitive, so "myName" and "MyName" are different names. 
* Variable names cannot include whitespace characters, math symbols, or arrows.

###### **Naming Conventions:** 
* Swift follows the camelCase convention for naming variables. 
* For constants and variables, camel case is used with a lowercase letter first (for example, "myName").
* For types and protocols, camel case is used with an uppercase letter first (for example, "MyName")
* Variables are first initialized by using "var".

### 2. Is your language statically or dynamically typed? 
##### Swift is statically typed. All information must be given to the compiler before compile time.

### 3. Strongly typed or weakly typed? 
##### Swift is strongly typed. It will always be sure to check that the variable is the correct type.

### 4. If you put this line (or something similar) in a program and try to print x, what does it do? If it doesn't compile, why? Is there something you can do to make it compile? x = "5" + 6 
##### Swift will not compile because 1. the variable isn't initialized with "var" and 2. because it is strongly typed, you cannot attempt to use a binary operand (+) to add a string and an int together. To fix it, we must make the numbers the same variable type. 
* Option 1: var x = "5" + String(6) OR var x = "5" + "6" - However, this will only make both numbers strings and place them together, so the output is "56", but it will still run.
* Option 2: var x = 5 + 6 OR var x = Int(5) + Int(6) - This will give the correct answer of 11.
