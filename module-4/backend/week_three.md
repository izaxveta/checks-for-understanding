## Week Three - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR.

1. At a high level, what is Node?
Node is an open source, cross platform JavaScript runtime environment. Essentially, it is JavaScript outside of the browser when previously JavaScript could only be run within the browser.

2. What is Express? What is Express similar to in the Ruby world?
Express is a fast, lightweight, unopinionated web application framework for Node.js. In the Ruby world, Express is similar to Sinatra, where it doesn't care about conventions very much so long as you string everything together. Also, Express is middleware.

3. How do we setup a route when creating an API with Node and Express? Please provide a code snippet.
Setting up a route when creating an API with Node and Express starts in the app.js file where you would define the route for a particular resource.

```JavaScript
var kittens = require('./routes/api/v1/kittens')
```
You would then continue to build out the directory structure for that specific resource within the routes directory.

4. What do we use Knex for?
Knex is a library that we use as a SQL builder to create queries in order to communicate with our database.

5. How **could** you organize your code to follow the MVC design pattern in your Quantified Self project?
You could organize your code to follow the MVC design pattern by adding model and controller directories to the parent directory. Within the model directory you would have files for each of the resources/objects that would be used throughout the applicatin and each would contain functions/methods applicable to the class/object. For the controller directory, there would be a contoller file for each of the routes and within each file would be action functions. Each of these action functions will define data that will be passed to and rendered in a view.

For'xample
```JavaScript
router.get('/', function(req, res, next) {
  kitten = {name: 'Sir FluffyButt'}
  res.render('kittens', {kitten: kitten})
})
```

6. How do you execute raw SQL in node?
```Node
database.raw('SELECT * FROM kittens')
```

7. What are some advantages to having your front end and back end code live in separate applications? What are some disadvantages?
Advantages of having front end and back end code live in separate applications include being more agile in swapping out components of the infrastructure for newer and better technologies, having front and back end applications means deploy strategies are wholly separate, allowing you to minimize disruption to user experience during deploys and focus on the right tool chains, and lastly, another advantage of having a front and back end live in separate applications is the ability to change the application at different paces.

Disadvantages of having front end and back end code live in separate applications involve the inability to take advantage of templating languages that frameworks may have, and having different strategies for build and deployment for both the front end and back end application - this may take up too much consumption of time and resources.

#### Review

8. Describe DNS.
DNS, or Domain Name Service, is the internet's system for converting aphabetic names into numeric IP addresses.

9. What does writing clean code mean to you?
To me, writing clean code means that variables are clearly and approprately named according to their values, methods abide by SRP and do not contain an excessive amount of lines, lines do not go beyond 80 characters, classes are clearly organized and only contain relevant properties and methods, variables are defined only to the appropriate scope in which they are to be used, and only the necessary information is utilized and passed around through methods/queries and nothing more.

10. If you were building an application that models hotels, what classes would you need? What classes would be responsible for what functionality? Hint: think about what tables you would need in the database, how those records would relate to each other, and good OOP.
If I were building an application that models hotels, I would have classes/tables for hotels, employees, rooms, and guests. Hotels would have many employees and employees would belong to a hotel. A hotel would also have many rooms to which a room would belong to a hotel. As far as guests, a guest has one guest room but could potentially have many guest rooms to which would call for having a table called hotel_guests which would create the relation between hotels and guests. A hotel has many guests and a guest could belong to many hotels.
