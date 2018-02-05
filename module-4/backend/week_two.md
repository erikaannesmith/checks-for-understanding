## Week Two - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. What's one difference between ES5 and ES6?
ES6 uses `const`,  `let`, and `=>`
2. What's the difference between asynchronous and synchronous JavaScript? 
synchronous javascript executes code one line at a time, asynchronous javascript jumps between tasks, but still works in a single-threaded way.
3. What are the four pillars of Object Oriented programming?
abstraction, encapsulation, inheritance, polymorphism
4. What are some tools available in JavaScript to help you write object oriented code?
constructors, prototypes, classes
5. What are some key concepts to be aware of when refactoring your JavaScript?
remove comments and debuggers, stay consistent on variable definition, mismatched semicolon usage
6. What's a callback function and what are some reasons when we use/need callback functions?
callbacks are functions passed through as arguments. we use them when we want to execute the function AFTER something else happens (asynchronous).
7. What's the scope of variables in Javascript?
if a variable is defined within the global context, it can be accessed anywhere. when it is defined within a function or block, it is only available within that scope. 
8. What's the difference between `==` and `===` in JavaScript?
`==` is loose equals, and `===` is strict equals. with loose equality, javascript will coerce the second value into the same object type as the first, then check if they are the same. with strict equality, if the values are not the same objects, it will return false.
9. Why do front end frameworks exist?
to maintain structure and keep code DRY.

#### Review  

10. Why do people say "HTTP is stateless"?
when you make a request, you have to pass through whatever instances you expect to persist, because the request itself does not hold onto those values.
11. Describe a RESTful API.
a RESTful API is one that accounts for all possible actions pertaining to an object (the ability to create, edit, view, or delete) and constructs them in an SRP way. It utilizes one action for each (get, post, put, patch, destroy)
12. What are some main characteristics of a team following an agile workflow?
the team would develop a plan for the immediate future, execute a small chunk of it (a `sprint`), and then develop their next plan based on their assessment of their progress from the prior sprint.
13. What are some advantages **and** disadvantages to using OAuth to authenticate a user?
OAuth saves the developer a lot of time and has built-in security, which would be difficult to manually maintain. However, your authentication process then becomes out of your hands, which means you don't have control over if the site you're authenticating through becomes hacked. It also ties your accounts together, which is not necessarily something the user wants. For example, if the user logs into your site with Facebook, other users then have access to their Facebook account.