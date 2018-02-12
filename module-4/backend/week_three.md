## Week Three - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. At a high level, what is Node?
Node is what we use to execute JavaScript in the terminal. It mocks V8's runtime.
2. What is Express? What is Express similar to in the Ruby world?
Express is the framework in which we write back-end JavaScript apps. It is similar to Sinatra.
3. How do we setup a route when creating an API with Node and Express? Please provide a code snippet.
We set it up by telling it WHERE to go ('/'), and where to look within the app for directions('foodsController.index')
`router.get('/', foodsController.index);`
4. What do we use Knex for?
Knex is how we connect with the database in Express
5. How could you organize your code to follow the MVC design pattern in your Quantified Self project?
We tried to focus on delegation of responsibility. Just as with Rails, we let the models handle the database calls and the controllers handled the status responses and anything other promises that needed to be made to serve up the information.
6. How do you execute raw SQL in node?
By calling `database.raw(<RAW SQL>)`
7. What are some advantages to having your front end and back end code live in separate applications? What are some disadvantages?
The main advantage seems to be separation of responsibilities. It is easier to know where to look for bugs when the front-end and back-end are separated. However, a disadvantage is that it definitely requires more work/time. It is a good idea for certain projects, and not for others. It depends largely on the scale of the project.

#### Review  

8. Describe DNS.
DNS is a protocol for how computers exchange data. It turns user-friendly domain names, like `www.facebook.com` into IP addresses so the request can be routed (it uses the IP address as an indentifier).
9. What does writing clean code mean to you?
Clean code is code that is both maintainable and scalable. It is single responsibility and implements pieces of code that could potentially be reused in other parts of the app.
10. If you were building an application that models hotels, what classes would you need? What classes would be responsible for what functionality?
You might want Room, Reservation, Hotel, Employee.
Hotels would have many rooms & employees, rooms would have many reservations.