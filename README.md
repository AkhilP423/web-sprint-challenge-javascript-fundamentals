# Sprint Challenge - JavaScript Fundamentals

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This challenge allows you to practice the concepts and techniques learned over the past week and apply them in project. This Sprint explored JavaScript Fundamentals. During this Sprint, you studied array methods, this keyword, prototypes, and class syntax. In your challenge this week, you will demonstrate proficiency by completing a range of JavaScript problems.

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the sprint challenge. 

## Introduction

The index.js file contains all of your challenges. Please review it in full before answering the questions. If you complete the stretch goals please leave them in your file but commented out so that they do not affect the MVP tasks 

In meeting the minimum viable product (MVP) specifications listed below, you should have all tests passing. You can console.log to check your work and ensure you are submitting the correct results 

### Commits

Set up codegrade early and commit your code regularly and meaningfully. 

## Interview Questions
### (please edit this file and write your answer below each question.)
Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read.

1. Explain the differences between `.map`, `.reduce` and `.filter` and describe a use case for each. 

    Before I explain, I want to see that Task 2 was quite annoying, and despite getting the right answer, codegrade didn't seem to like the way I formatted the function. I know that it's on me for not fulfilling the requirement, but I feel as though human eyes should uncomment the console.logs that I commented and see for yourself, and at least consider partial credit if it's deserved. Thank you!

    .map() is an iterator function that is used for manipulating or reshaping data. It returns a brand new array without touching the original array. Whatever you set the function call equal to, you can map it to the new array. A use case for .map is replacing a for loop that loops through an object to set a certain part of the object into a new array. For instance, a set of objects with cities and states can be looped through to form a new object with just the cities, with the .map function.

    .filter() is similar to .map, returning a new array and calls back each element, index, and returns each in turn. However, .filter() initiates a "truth" test, and only returns the elements if true, else ignores. It's instead used for filtering out an array by a specific condition. A use case may be to filter out a bunch of students' grades in an array, and push only students' data that receive a '70' as their grade, in order to list everyone who passed.

    .reduce() method is used to execute a reducer function on each value of the array it's attached to. It returns a single value which is the accumulation of the reducer function. Since it only returns a single value, it is vastly different in use cases from .map or .filter. A good use case would be to .reduce() a data set with several integers, such as state population to find the total sum (giving you the country population).

2. Explain the difference between a callback and a higher order function.
    A higher order function takes another function (or functions) as an arguments and returns a function to its callers. A callback function is a function that is passed to another function, in order to be called by said function. Thus, a callback function is not necessarily a higher order function, but a function that receives a callback as an argument is a higher order function.

3. Explain what a closure is.
     A closure is a function bundled together with references to the surrounding state. Essentially, it gives you access to an outer function's scope from an inner function. Closures are created every time a function is created, upon creation.

4. Describe the four principles of the 'this' keyword.
    1. Window binding - If 'this' isn't given any context, it will return the window, the global object in the node terminal. It is undefined in strict mode.
    2. Implicit Binding - In objects with methods, when the function(method) is invoked, 'this' refers to what is on the left of the dot.
    3. Explicit Binding - We can explicitly tell a function that 'this' should be using .call, .apply, or .bind. Call invokes the function and passes arguments 1 by 1. Apply invokes the function and passes arguments as an array. Bind passes arguments 1 by one but does not immediately invoke the function, and returns a new function to invoke later.
    4. New Binding - If a function is invoked with a new keyword, the 'this' inside said function is bound to the new object constructed. If a function is invoked as a constructor function using the new keyword, 'this' again points to the new object created.

5. Why do we need super() in an extended class?
  The super keyword refers to the parent class. It must be used to call the constructor of said parent to access the parent's properties and methods.

## Instructions

### Task 1: Set up Project

Using VSCode and Command Line:


1. Fork the repo
2. Go into canvas and connect your reop to codegrade
3. Clone your forked version of the repo
4. DO NOT CREATE A BRANCH. You will be pushing your changes to the main/master today
5. cd into your repo
6. open the terminal in your vs code and type `npm install`
7. next type `npm run test` in your terminal
8. Complete your work making regular commits to main/ master your codegrade score will update each time you make a push.


### Testing & Debugging

Open a second terminal inside of your project by clicking on the split terminal icon
![alt text](assets/split_terminal.png "Split Terminal")

Inside of your second terminal type `npm start` 
![alt text](assets/npm_start.png "type npm start")

You will be running your tests in one terminal and debugging in the other. As you work on your code you should make use of `console.log` to check your progress and debug.
![alt text](assets/tests_debug_terminal_final.png "your terminal should look like this")

### Task 2: Project Requirements (MVP)

You must complete all tasks inside of `index.js` and answer the questions above.

In your solutions, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

## Resources
 
 [Sprint Challenge Study Guide](https://www.notion.so/lambdaschool/Unit-1-Sprint-3-Study-Guide-033a9a00659a4ef98c12eb97e49a6110)

## Submission format

Please submit your project via codegrade by following [these instructions](https://lambdaschool.notion.site/lambdaschool/Lambda-School-Git-Flow-Step-by-step-269f68ae3bf64eb689a8328715a179f9) See part 2, submitting an assignment with codegrade
