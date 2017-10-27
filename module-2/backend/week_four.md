## Week Four Recap

### Instructions
Fork this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

* What is a cookie?

Client-side data from the server.

* What’s the difference between a session and a cookie?

Sessions are stored on the server
Cookies are stored on the browser.

* What’s a flash and when do you want to use flashes?

Flash is a temporary notification sent to the user when they do a specified thing.
You want to use them to alert the user that they have interacted somehow with CRUD functionality of an object (created, edited, viewed, or deleted).

* Why do people say “HTTP is stateless”

Because the connection between the browser and the server is lost at the end of the session.

* What’s authentication? Explain.

Authentication is checking if you are who you say you are (a superstar).

* What’s the difference between authentication and authorization?

Authorization deals with accessibility (are you allowed to be here?)

* What’s a before filter?

A tool used to organize your controller by extraction of information regarding authorization and authentication.

* How do we keep track of a user once they’ve logged in?

Sessions.

* When do you want to namespace a resource? When do you want to nest a resource? What's the differences between those two approaches?

Admin has no resources - namespacing is a good option for authentication of different user/roles.
Nesting is a good option when both objects have resources.

* At a high level, what tools can you use to implement authorization? How would you use them?

-allow_any_instance_of to stub a method
-using enums for some additional methods/readability
-using a namespace to organize things
-using before action to check a user's status
-using inheritance to help refactor

* What's an enum, and what advantages does it offer? What data type needs to be in your database to use an enum? Where do you declare an enum?

An enum is a tool used to translate the roles, input as integers, into strings. So the data type in the database needs to be an integer.
You declare an enum in the model.

* What are some strategies you can use to keep your views DRY?

Partials!
