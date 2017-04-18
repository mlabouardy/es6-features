# Scopes

javascript is function scoping not block scoping, in java to create a block we use {}, in js we use function

global variables are bad -> all scripts in a web page execute in common namespace
you dont want a global variable to clash with another global variable in another script

IIFE = Immediatly Invoked Function Expression (its a way to call anonymous function):

```
(function (){
 var a = 4;
 var b = 3;
 console.log(a+b);
})()
```

- JS is compiled & interpreted language
- JS is single threaded
- Undecalared variable(without var keyword) is registred to the global scope when we do a write operation

## Hoisting

Concept in JS: moving declarations to the top

## Strict Mode

"use strict"

- prevent write operation on undeclared variables

## Closures

function which remembers its scope even

its a way to make private variables (module pattern)
