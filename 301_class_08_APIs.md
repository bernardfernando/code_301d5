Reading
[API Design Best Practices]link did not work

## What does REST stand for?

_Representational State Transfer(REST) is software achitecture that imposes conditions onhow an API should work. It was initially created as a guideline to manage communicaiton on a complex network like the internet._

## REST APIs are designed around a resources, _which are any kind of object, data or service that can be accessed by the clent. REST APIs use uniform interface, which helps to decouple the client and service implementations._

## What is an identifier of a resource? Give an example.

_Uniform Resource Identifier - host name and port number._

## What are the most common HTTP verbs?

_Methods - POST, GET, PUT AND DELETE: there create, read, update and delete operations respectively._

## What should the URIs be based on? _Resource Description Framework(RDF) - Web Ontology Language (WOL) - and they have unique indivisual identifiers._

## Give an example of a good URI. _URL_

## What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

_Any API that requires more than a single call to perform a single common operaiton.\_It is not healthy to have Chatty APIs._

## What status code does a successful GET request return?

_200 OK._ (2xx)

## What status code does an unsuccessful GET request return? _404 (4xx)_

## What status code does a successful POST request return? _200 OK (32xx)_

## What status code does a successful DELETE request return? _200 OK_

Bookmark and Review
[RegExr](https://regexr.com/) - Pay particular attention to the cheatsheet
[Regex Tutorial](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285)
[Regex 101](https://regex101.com/)

## Cheatsheet

Character classes
. any character except newline
\w\d\s word, digit, whitespace
\W\D\S not word, digit, whitespace
[abc] any of a, b, or c
[^abc] not a, b, or c
[a-g] character between a & g
Anchors
^abc$ start / end of the string
\b\B word, not-word boundary
Escaped characters
\.\*\\ escaped special characters
\t\n\r tab, linefeed, carriage return
Groups & Lookaround
(abc) capture group
\1 backreference to group #1
(?:abc) non-capturing group
(?=abc) positive lookahead
(?!abc) negative lookahead
Quantifiers & Alternation
a\*a+a? 0 or more, 1 or more, 0 or 1
a{5}a{2,} exactly five, two or more
a{1,3} between one & three
a+?a{2,}? match as few as possible
ab|cd match ab or cd
