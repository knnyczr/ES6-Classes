# ES6 Classes

JavaScript classes is what developers call Syntactical Sugar. 
It makes JavaScript a little easier or "sweetens" over JavaScript's existing protype-based inheritance. 

## Objects

We know how to declare a variable, give it key:value pairs. and we know how to give those objects methods

```javascript

let student = {
    fname: 'kenny',
    lname: 'cruzer',
    speak(){
        return(
            `Hey I\'m ${this.fname} ${this.lname}`
        )
    }
}

console.log(student.speak())
// expected output => Hey I'm kenny cruzer

```

----

Classes are just like JavaScript functions, you can define them either with an expression or declaration. 

[Class Expression](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/class) VS [Class Declarations](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/class)

The `constructor` method is a special method for creating and initializing an object created with a `class`. There can only be one! – per class, else a syntax error. 


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

## this

`this` is a special key word that refers to the instance of the the class in that point in time. It refers to current object you're talking about. We'll get back to what this means after. 

## Doggo

* So let's create a Class for our dogs, that creates objects with a breed, a first name, and an age. 

* In our magical land of speaking dogs, we're going to write a method that will have our dog speak

* Unfortunetly for us, dog's mature and age much faster than humans do, their life spans are much shorter. We're also going to create a method that converts our dog's years into human years. 


```javascript

class Dog {
    constructor(breed, fname, age){
        this.breed = breed; 
        this.fname = fname; 
        this.age = age; 
    }
    speak(){
        console.log(
            `My name is ${this.fname}, 
            I am ${this.humanYears()}, 
            and I am a ${this.breed}`
        );
    }
    humanYears(){
        return this.age * 7; 
    }
}

```

Easy right? Well we only created the cookie cutter for our dogs. But this class is very powerful. It declares object instance, and the objects will have three things at 'birth:' a breed, a first name and an age that describes that instance of a dog. The dog you create also has 2 'abilities' or methods. It can `speak()` and it can rephrase it's age into `humanYears()`



## Create your own Dogs!

* touch a new file, in this repo name it dogs.js and be prepared to run it with node in the terminal
* Make your own imaginary dogs, tell them what kind of breed they are, give them a first name and tell them how old they are, and give them the ability to convert its age into human years. 

CHALLENEGE: 
* Create a method for when these adorable dogs are adopted, have the method accept a *string* to *rename* the dog. 

## Create a for cars

* touch a new file, in this repo name it cars.js and be prepared to run it with node in the terminal
* Make a class for cars, tell me what brand these cars can be, give them a color, give them a year, 
* make it `honk()` and console.log all of it's attributes. 
* Give it one more method to change it color. 

