## Week Two - Module 4 Recap

Note: When you're done, submit a PR.

1. What's one difference between ES5 and ES6?
One difference between ES5 and ES6 is the syntax.
This is ES5 syntax for a function:
```JavaScript
.map( function ( ) {
// Code goes here
})
```

ES6 is as follows:
```JavaScript
.map( ( ) => {
// Code goes here
}
```

2. What's the difference between asynchronous and synchronous JavaScript?
Synchronous JavaScript is when one block of code must finish running before your application can continue processing. Asychronous JavaScript is when your application can continue running while other threads are still being processed.

3. What are the four pillars of Object Oriented programming?

The Four Pillars of Object Oriented programming are:
- Abstraction
- Encapsulation
- Inheritance
- Polymorphism

4. What are some tools available in JavaScript to help you write object oriented code?
Some tools available in JavaScript to write object oriented code include classes, prototypes, inheritance and constructors.

5. What are some key concepts to be aware of when refactoring your JavaScript?
Some key concepts to be aware of when refactoring JavaScript is the understanding of why and how the code would need to be refactored, what rules or conventions it violates, any headaches the code has introduced to the project, how it might be refactored or dealt with and why refactoring would be worth the time and effort.

6. What's a callback function and what are some reasons when we use/need callback functions?
A callback function, also known as a higher-order function, is a function that is passed into another function as a parameter, and the callback function is called inside the function.

7. What are the different scopes of variables in Javascript? When would you want to define global variables?
In JavaScript, there is local as well as global scope. One would typically want to define global variables when information should be accessible throughout the space in which it's defined, including inside other functions existing in the same space.

8. What's the difference between `==` and `===` in JavaScript?
While both are relational operators ==, or loose equal, checks to see is something is equal to the other. ===, or strict equal, also checks to see if something is equal to ther other but it also compares the TYPES of both values.

9. Why do front end frameworks exist?
Frameworks exist to provide additional features and benefits that assist the developer when building and designing applications. In the case of JavaScript, a language that currently leaves much to be desired as a standalone language, there are many frameworks (and libraries) available to help developers with their many 'wants'.

#### Review

10. Why do people say "HTTP is stateless"?
HTTP is referred to as stateless protocol due to the fact that each command is a request and executed independently, without any knowledge of the request that were executed before it. A stateless protocol does not requre the server to retain information or status about each other fo the duration of multiple requests.

11. Describe a RESTful API.
A RESTful API uses HTTP requests to GET, PUT, POST and DELETE data. Based on representational state transfer technology, an architectural style and approach to communications often used in web services development. It leverages less bandwith making it more suitable for internet usage.

12. What are some main characteristics of a team following an agile workflow?
Some main characeristics for a team following an agile workflow revolve around collaboration and continuous improvement. An agile team also exemplifies daily communication, teamwork, problem solving, technical development skills and the determination to improve the team's velocity with each iteration.

13. What are some advantages **and** disadvantages to using OAuth to authenticate a user?
## Some advantages of using OAuth include:
### From a user perspective:
- Third party handling user authentication - Privacy, security and control of not sharing your information to too many parties.
- It saves time. No need for the user to go through the process of creating yet another account.
### From an application perspective
- Accessibility to additional user information provided and allowed by the authenticator.

## Some disadvantages of using OAuth:
### From a user perspective
Risk of having the main account that is associated with all other accounts compromised.
### From both a user and applicatino perspective
Third party is handling user authentication - possible data misuse.
Some users may not have an account with whom you're allowing to handle authentication.
