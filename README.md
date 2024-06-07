# JAVASCRIPT-Errors
JavaScript errors are objects. </br>
  Contains properties: Name and message </br>

###### To create errors and send to a user we can use the Error function. <br> 
   It allows us to make an error object with a message that is unique to an error you want to convey! </br>
   
    console.log(Error('Your password is too weak.'));    //Error(create error objects) { message: 'Your password is too weak.'}
    console.log(new Error('Your password is too weak.'));    //Using new  

###### However to actually throw an error we must use the throw keyword</br>

     throw Error('Something wrong happened/MESSAGE HERE');              //throws error object </br>
           // Error: Something wrong happened</br>
      console.log('This will never run');</br>
           // Code after the throw statement will not execute (PROGRAM STOPS RUNNING WITH THROW)</br>

###### To anticipate and handle errors and allow a program to run:</br>
We use try...catch() and a throw statement (Similar to Error() but won't stop program). </br>

      try {                                           //Try block contains code that might throw error
        throw Error('This error will get caught');        //throw an error 
      } catch (e) {                                  //Catch block catches the error
        console.log(e);                              //if code in try has error it handles the error
      }
      // Prints: This error will get caught
      
##### // try...catch Throws a JS engine (compiler) built-in Errors [Type, Syntax, Reference...]
###### Built-in Errors are Run-time Errors

     try {
           The code can throw built-in errors like syntax, reference, type
           which is caught by the JS engine
     }
     catch {
           catch can still handle the error for us
     }
##### // Example try...catch statement that throws a built-in error     
     
     const fixedString = 'Cannot be reassigned';
     try {
       fixedString = 'A new string'; // A TypeError will be thrown (JS BUILT IN ERROR)
     } catch (e) {
       console.log('An error occurred!'); // Prints 'An error occurred!'
     }
     console.log('Prints after error'); // Program continues running after the error is handled and prints 'Prints after error'
     'An error occurred!'
     'Prints after error'
     
## The Error Object
Contains information about the thrown exception. </br>
The information is found in 2 properties:  </br>

1. `Name` Sets or returns an error name. (Type of Error)  </br>
2. `Message` Sets or returns an error message. (Description of instance.)  </br>


All error types along with their properties are inherited from the Error object. </br>
Think of it like a pyramid. </br>
Error is at the top, followed by the different types of errors, </br>
then finally by their properties.</br>

| | | Error |  | |
|-------|-------|------|------|------|
| “ReferenceError” | “SyntaxError” | “TypeError” | “EvalError” | “URIError” |
| Type of Errors Properties | Type of Errors Properties | Type of Errors Properties| Type of Errors Properties | Type of Errors Properties |

## Errors returned by the Name property:

|Error Name or Type of Error| Description | How to fix by Checking | 
|-------|-------|------|
| “EvalError” | An error has occurred in the eval() function (Note: Depreciated in newer versions of JavaScript) |
| “RangeError” | A number “out of range” has occurred | |
|“ReferenceError” | Using a variable that doesn't exist | Properly declare of variables or create new |
|| code after Reference Errors will not work|
| “SyntaxError” | Syntax error a typo creates invalid code| opened/closed brackets, braces, parentheses, semicolons |
| “TypeError” | Perform an operation on a value of incorrect type | Used a String method on a number/ so use a method for #'s |
| “URIError” | An error in encodeURI() has occurred | |
| “Internal” |  | |

###### “TypeError” example: 

    const reminder = 'Reduce, Reuse, Recycle';
    reminder = 'Save the world';
    //// TYPE ERROR: RE ASSIGNMENT TO A CONSTANT VARIABLE./////
    //// CODE AFTER WILL NOT COMPLETE./////
    console.log('This will never be printed!');
    
###### Additional Examples:

    function areaOfCircle(radius) {
      return pi * radius * radius;
      // : correct answerReferenceError: pi is not defined
    }
    const radius = 3;
    console.log(areaOfCircle(radius);
    // : correct answerSyntaxError: missing ) after argument list
                
    radius = 5;
    // : correct answerTypeError: Assignment to constant variable.
 
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


  



  
