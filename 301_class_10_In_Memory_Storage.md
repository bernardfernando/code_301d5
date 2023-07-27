Readings: In memory storage
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

What is a ‘reference error’?
What is a ‘syntax error’?
What is a ‘range error’?
What is a ‘type error’?
What is a breakpoint?
What does the word ‘debugger’ do in your code?
Bookmark and Review
JavaScript errors reference on MDN
