## Week One - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR.

1. What's the most useful thing you learned from completing the intermission week work?
The most useful thing I learned from completing the intermission week work was going through the JavaScript fundamentals. It was useful to go over the material, run through the lessons exercises, and take notes. I didn't have the opportunity to get to any of the extensions but I think going through additional exercises like the homework from the first week would have me feeling more confident in JavaScript. I had even thought about doing front-end Mythical Creatures.

2. What are some tools to help debug JavaScript code?
Some tools I was previously utilizing to help debug JavaScript code include the use of `console.log()` to see what return values I get from functions and variables, `eval(pry.it)` (also, `debugger;`). After Friday's lesson I found that Chrome's developer tools (Element, Console, Source and Network tabs) are also very useful in assisting in JavaScript debugging and expanding my understanding of the performance of my applications.

3. What are some tools you need in order to unit test your JavaScript?
Some tools needed in order to unit test JavaScript are Mocha and Chai. Mocha is used for running tests and provieds `describe()`, `context()` and `it()` functionality, while Chai is a popular assertion library.

4. What is the syntax for invoking a function? Give an example.
You may have a function called `adoptCat` which does x, y and z. Simply calling `adoptCat` in the console will return that it is a function, but that function will not be invoked unless it is called like so: `adoptCat()`

5. What's `this` in JavaScript?
JavaScript's `this` refers to the parent object, and is dependent on the context in which it was referenced. When used in the global context, `this` refers to 'document' or 'window'. In the context of an object, `this` refers to and is boud to the object itself.

6. What is Webpack and why is it useful?
Webpack is a Node package that inspects our asses, finds dependencies, and creates a JS file (main.bundle.js) that is used for production.

7. When/why do you want to use event delegation?
Event delegation involves taking advantage of the fact that events bubble in the event loops by setting an event listener on one parent. This event listener analyzes bubbled events to match its child elements.

One may want to use event delegation to prevent the possibility of setting mutiple listeners on the same node. Also, as was shown in class, event delegation is useful as event listeners are only applied to objects that are present within the HTML document when the script is loaded. If one applies event listeners to `li` objects but new `li` objects are added after the page has loaded, event listeners will not be connected to those new `li` objects as the script has already been run.

8. What's `npm` and what do we use it for?
`npm` is a Node Package Manager (hence n.p.m.) that allows for organization of outside packages much like Ruby Gems.

#### Review
9. What's the MVC design pattern? Describe each part of MVC.
The MVC is a design pattern that revolves around Models, Views, and Controllers.
Models are objects that are sometimes POROs, but often represent and define the blueprint data and relationships that exist in a database. Views are html/erb files that render information to the viewer in the browser. The information that is rendered is dependent on the data that is sent to it from the Controller, which is the mediator between the Models and Views.

10. What are a few ways to optimize a Rails application?
A few ways to optimize a Rails application is to incorporate tools like New Relic to find where that application can be modified to increase data load speeds, incorporate background workers, optimize queries to use indexes and methods that obtain only information that we need and nothing more, Redis for caching, etc.

11. What's a background worker? When would we want to use a background worker?
A background worker is a concept that is used to help optimize your application. Background workers are often used for sending data emails to users for tasks that may take a while - so rather than the user waiting for the information to be parsed and the page to be loaded, the user is immediately redirected to another page and notified that when the task is complete that an email will be sent. This way, the user can continue navigating through the application and will not be held up by waiting for a task to be completed.