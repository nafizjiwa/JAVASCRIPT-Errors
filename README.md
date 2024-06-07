# JAVASCRIPT-Errors
Javascript throughs errors as an object. </br>

The errors are caught by a catch block of a try...catch or by a throw statement. </br>

## The Error Object
Contains information about the thrown exception. </br>
The information is found in 2 properties:  </br>

1. `Name` Sets or returns an error name. (Type of Error)  </br>
2. `Message` Sets or returns an error message. (Description of instance.)  </br>

## Errors returned by the Name property:

|Error Name or Type of Error| Description | How to fix by Checking | 
|-------|-------|------|
| “EvalError” | An error has occurred in the eval() function (Note: Depreciated in newer versions of JavaScript) |
| “RangeError” | A number “out of range” has occurred | |
|“ReferenceError” | An illegal reference to a variable | Properly declare of variables | |
| “SyntaxError” | Syntax error a typo creates invalid code| opened/closed brackets, braces, parentheses, semicolons |
| “TypeError” | An operation done on value of the wrong type | String method on a number use differnt method |
| “URIError” | An error in encodeURI() has occurred | |
 
## Mesages for various errors:
|Error Name or Type of Error| The Message Provided |
|-------|-------|
| RangeError|  invalid array length |
| |  invalid date|
| ReferenceError |  “x” is not defined |
|| assignment to undeclared variable “x” |
| SyntaxError | “x” is a reserved identifier |
||  a declaration in the head of a for-of loop can’t have an initializer |
| TypeError |  “x” is not a function |
||  “x” is read-only |
| URIError| malformed URI sequence |


  



  
