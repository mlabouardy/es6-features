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

## Read vs Write operations

