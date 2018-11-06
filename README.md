# ES6 Classes

JavaScript classes is what developers class Syntactical Sugar. 
It makes JavaScript a little easier or "sweetens " over JavaScript's existing protype-based inheritance. 

Classes are in fact JavaScript functions, you can define them either with an expression or declaration. 

[Class Expression](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/class) VS [Class Declarations](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/class)

The `constructor` method is a special method for creating and initializing an object created with a `class`.


## Class Expressions
Much like function expressions you can define them with a variable to initialize it, use the contructor key word and boom.

```javascript

let dog = class { 
    constructor(breed, age){
        this.breed = breed; 
        this.age = age; 
    }
}

console.log(dog.name)
// expected output => dog

let dog = class doggo{ 
    constructor(breed, age){
        this.breed = breed; 
        this.age = age; 
    }
}

console.log(dog.name)
// expected output => doggo

```

## Class Declarations
Much like function declarations you can define them by using the class keyword, a name, and the constructor keyword to initialize your `class`. 

```javascript

class Dog {
    constructor(breed, age){
        this.breed = breed; 
        this.age = age; 
    }
}

```