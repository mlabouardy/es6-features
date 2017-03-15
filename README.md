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

We can even minimize the code above

```
let circleArray = x => x*x*3.14;
```

## Template literals

Its a way to concat variable inside a string

```
let name = 'Mohamed'
let age = 23
let output = `My name is ${name} and I'm ${age} years old`
console.log(output) // My name is Mohaemd and I'm 23 years old
```

## Spread operator

Split an array

```
function add(a,b,c){
  return a+b+c;
}

var l = [1,4,6];
add(...l);
```
## Classes

```
class Person{
  constructor(name, age){
    this.name = name;
    this.age = age;
  }
  
  getName(){
    return this.name;
  }
  
  getAge(){
    return this.age;
  }
  
  whoIam(){
    return `My name is ${this.name} and I'm ${this.age} years old`
  }
}
```

To instanciate an person object

```
let mohamed = new Person('Mohamed', 23);
console.log(mohamed.getName()); // Mohamed
console.log(mohamed.getAge()); // 23 
console.log(mohamed.whoIam()); // My name is Mohamed and I'm 23 years old
```

## Inheritance

```
class Animal {
  constructor(name){
    this.name = name;
  }
  
  eat(){
    console.log('Eating ....');
  }
}

class Rabbit extends Animal{
  f(){
    console.log('Calling f function');
  }
}

class Lion extends Animal{
  g(){
    console.log('Calling g function');
  }
}
```
