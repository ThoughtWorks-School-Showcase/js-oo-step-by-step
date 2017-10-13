# Object-Oriented Programming Basic

## Business Requirements:
### Practice 1
Declare a class called `Person` with properties `name` and `age`, and a method called `introduce`, the method should return a string:
`My name is Tom. I am 21 years old.`

Declare class `Student` which should be subclass of `Person`. Except `name` and `age`, a student should have a class property(you should name it `clazz` because `class` in a keyword in JavaScript). It should also have an `introduce` method which returns a string:
`My name is Tom. I am 21 years old. I am a Student. I am at Class 2.`

Declare a `Worker` class derived from `Person` which only have `name` and `age`,  it also has an `introduce` method which returns a string:
`My name is Tom. I am 21 years old. I am a Worker. I have a job.`

All these three sentences below:
`My name is Tom. I am 21 years old.`
Should write only once in the code, it should be placed in `Person`’s introduce method.

### Practice 2
Declare `Person` class with `id`, `name` and `age` in *prototype* manner, use `id` to identify different person. It has an `introduce` method which returns a string:
`My name is Tom. I am 21 years old.`

Declare `Student` class derived from `Person`,  except `id`, `name` and `age`, it has a `class` property. Student also has an `introduce` method which returns a string:
`My name is Tom. I am 21 years old. I am a Student. I am at Class 2.`

But the `class` property is not a number but an object, write a `Class` class with property `number` and `leader`, and property `leader` should not appear in constructor.

Refer to the test cases, you should pass a `Class` object when construct a Student. The Class has a method called `assignLeader` which receives a Student as parameter. It means to assign the Student as the class leader. When Tom is a class leader, call`tom.introduce()` should return a message:
`My name is Tom. I am 21 years old. I am a Student. I am Leader of Class 2.`
If Tom is not a class leader, return the old message.

Declare `Teacher` class as subclass of `Person`, it has a `classes` property except `id`, `name` and `age`. It’s `introduce` method return a string:
`My name is Tom. I am 21 years old. I am a Teacher. I teach Class 2,3.`

When `classes` is empty, it returns:
`My name is Tom. I am 21 years old. I am a Teacher. I teach No Class.`

The string below of all subclasses of `Person` class should be from `person.introduce()`:
`My name is Tom. I am 21 years old.`

### Practice 3

Base on `practice 2`, fulfill the following requirement:

Add method `appendMember` in class `Class` which receive a student instance as parameter, means append this student to the class.

If a student is belongs to a class, when call `assignLeader`, it should succeed and print:
`Assign team leader successfully.`

If the student is not is the class, `assignLeader` should fail and print:
`It is not one of us.`

Of course `student.introduce()` should return:
`My name is Tom. I am 21 years old. I am a Student. I haven't been allowed to join Class.`
To determine whether a student belongs to a class, there should have a `hasStudent` in `Class` class.

Teacher has a method `isTeaching`, receive a student as a parameter and return a boolean value. If the student belongs to any classes which the teacher is teaching, it represents the teacher is teaching the student.

When a student join a class, the teacher who is teaching the class should print:
`I am Tom. I know Jerry has joined Class 2.`

When a student is assigned as a class leader, the teacher who is teaching the class should print:
`I am Tom. I know Jerry becomes Leader of Class 2.`

## Practice Challenges:
* Apply ES6 OO feature 
* Declare class in `prototype` manner
* Extend a class
* Override a method in the parent class
* Simple OO implementation via Javascript

## Practice Requirements:
* Pass all tests
* Commit frequently with readable commit comment via Git
* Coding with keyboard shortcuts

## Practice Output:
Modify code under `main` directory to pass all tests under `spec` directory according to the requirements.

## Environment
Node Js
NPM

## How to begin：
Open your terminal, change to any path and clone this repository:
```
git clone `this repo site`
```
Install dependencies:
```
npm install
```
Run all tests:
```
npm test
```
Run specific test:
```
node_modules/jasmine/bin/jasmine.js spec/section-1/practice-1-spec.js
```
You can find these two key folders when you open the repository with your favorite code editor:
```
spec  //Test code, stands for specifications
src   //Source code
```

## Learning Resource
1. [JavaScript Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics)
2. [JavaScript Code Camp](https://www.freecodecamp.org/challenges/comment-your-javascript-code)
3. [JavaScript Objects](https://www.w3schools.com/js/js_objects.asp)
4. [ECMAScript 6 Features](http://es6.ruanyifeng.com/)
5. [Install Node](https://github.com/creationix/nvm)
6. [Install NPM](https://github.com/npm/npm)
7. [Jasmine Tutorial](http://jasmine.github.io/2.4/introduction.html)
8. [Git Reference](https://git-scm.com/docs)
9. [Array](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array)