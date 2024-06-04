# JAVASCRIPT-Errors
Javascript throughs errors as an object. </br>

The errors are caught by a catch block of a try...catch or by a throw statement. </br>

## The Error Object
Contains information about the thrown exception. </br>
Where information? In its 2 properties:  </br>

1. `Name` Sets or returns an error name. (Type of Error)  </br>
2. `Message` Sets or returns an error message. (Description of instance.)  </br>

Errors returned by the Name property:
|Error Name| Description |
|-------|-------|
| “EvalError” | An error has occurred in the eval() function (Note: Depreciated in newer versions of JavaScript) |
| “RangeError” | A number “out of range” has occurred |
|“ReferenceError” | An illegal reference has occurred |
| “SyntaxError” | A syntax error has occurred |
| “TypeError” | A type error has occurred |
| “URIError” | An error in encodeURI() has occurred |

Mesages for various errors:

RangeError
  invalid array length
  invalid date
ReferenceError
  “x” is not defined
  assignment to undeclared variable “x”
SyntaxError
  “x” is a reserved identifier
  a declaration in the head of a for-of loop can’t have an initializer
TypeError
  “x” is not a function
  “x” is read-only
URIError
  malformed URI sequence
