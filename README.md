# ES6 Features

## let keyword

Define the scope of a variable:

```
function getName(){
  let name = 'Mohamed'
  return name;
}

console.log(getName()); // Mohamed
console.log(name); // Error undefined
```
A variable declared with the "let" keyword can be used inside the block of declaration (between curly braces)

## Arrow functions

Its a way to write functions without the keyword "function"

- Before

```
function circleArray(x){
  var PI = 3.14;
  return x*x*PI;
}
```

- After

```
let circleArray = (x) => {
  const PI = 3.14;
  return x*x*PI
}
```
