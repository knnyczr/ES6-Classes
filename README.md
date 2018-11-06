# ES6 Classes

JavaScript classes is what developers class Syntactical Sugar. 
It makes JavaScript a little easier or "sweetens " over JavaScript's existing protype-based inheritance. 

Classes are in fact JavaScript functions, you can define them either with an expression or declaration. 

[Class Expression](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/class) VS [Class Declarations](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/class)


## Class Expressions
```javascript

let dog = class { 
    constructor(breed,name){
        this.breed = breed; 
        this.name = name; 
    }
}

```