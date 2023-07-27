# In memory storage

Below you will find some reading material, code samples, and some additional resources that support the topic for this class and the upcoming lecture.

Review the Submission Instructions for guidance on completing and submitting this assignment.

Reading
[Understanding the JavaScript Call Stack](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4)

## What is a ‘call’?_The call stack is primarily used for function invocation (call)._

## How many ‘calls’ can happen at once?

_Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous._

## [What does LIFO mean?] _Last in First Out_

_LIFO: When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns._

## Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

function firstFunction(){
throw new Error('Stack Trace Error');
}

function secondFunction(){
firstFunction();
}

function thirdFunction(){
secondFunction();
}

thirdFunction();

## What causes a Stack Overflow?

_A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error._

Here is an example:

function callMyself(){
callMyself();
}

callMyself();
The callMyself() will run until the browser throws a “Maximum call size exceeded”. And that is a stack overflow.

JavaScript error messages

## What is a ‘reference error’?

_This is as simple as when you try to use a variable that is not yet declared you get this type os errors._

_console.log(foo) // Uncaught ReferenceError: foo is not defined
This is also a common thing when using const and let, they are hoisted like var and function but there is a time between the hoisting and being declared so when you try to access them a reference error occurs, the fact that this happens to let and const is called Temporal Dead Zone (TDZ)._

_foo = 'Hello' // Uncaught ReferenceError: foo is not defined_
let foo\_
_Whatever you are using (var, let or const) the fix is as simple has declaring the variable before any declaration is made._

**let foo;**
**foo = 'Hello'**

## What is a ‘syntax error’?

_I know it’s in the name of the errors, but like it says itself, this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse._

_JSON.parse( {'foo': 'bar'} ) // Uncaught SyntaxError: Unexpected token o in JSON at position 1_
_This can be solved by just fixing the syntax, in this case the object should be a JSON._

_JSON.parse('{"foo":"bar"}')_
_Some syntax errors like sending a trailing comma when calling a function are handled without error by most recent browsers, but older ones you have to be careful._

## What is a ‘range error’?

_Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up._

_var foo= []_
_foo.length = foo.length -1 // Uncaught RangeError: Invalid array length_
_An array for instance cannot have a negative length, why would you mess with the array length? Some people use it to set an array to empty, something of the likes of:_

_var foo = [0, 0]_
_foo.length = foo.length - 2 // (or foo.length - foo.length)_
foo // would log [] instead of [0, 0]\_

## What is a ‘type error’?

_Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable._

## What is a breakpoint?

_To check if a program works upto a point, which is called a breakpoint. This can be done by simpliy clicking on the number of the porgrame line where you want to stop to taking account upto that point_
_This can also be achieved by having a debugger statement in your code. eg i === 30._

## What does the word ‘debugger’ do in your code?

_Removing errors or 'bugs' from the program._

Bookmark and Review
[JavaScript errors reference on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)
