## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!).

Note: When you're done, submit a PR.

1. List the five common HTTP verbs and what the purpose is of each verb.

- Get: Read
- Post: Create
- Put: Update
- Patch: Update
- Delete: Destroy
* Difference between put & patch: Patch is for PART of an entry, put is for the entire entry.

2. What is Sinatra?

Sinatra is a DSL in Ruby for writing web apps.

4. What is MVC?

MVC is model-view-controller.

5. Why do we follow conventions when creating our actions/path names in our Sinatra routes?

To ensure that all possible user routes are covered.

6. What types of variables are accessible in our view templates without explicitly passing them?

Instance variables.

7. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template?

  ```ruby
  get '/horses' do
    @count = 1
    erb :index
  end
  ```

8. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed` to the view?

name = "Mr. Ed"

9. What's the purpose of ERB?

ERB files are embedded ruby and combine text with ruby to produce a web page.

10. Why do I need a development AND test database?

So we don't have to worry about data in our development database.

11. What is CRUD and why is it important?

C - Create
R - Read
U - Update
D - Destroy
These are important because they ensure that we create restful routes.

12. What does HTTP stand for?

Hypertext Transfer Protocol

13. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways?

<% %>, which runs the line
or <%= %>, which runs and returns the value of the line (expects an output)

14. What's an ORM?

Object Relational Mapping - turns data pieces into objects so we can manipulate them.

15. What's the most commonly used ORM in ruby (Sinatra & Rails)?

ActiveRecord.

16. Let's say we have an application with restaurants. There are seven verb + path combinations necessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.

- get '/restaurants' : Shows index of all restaurant entries
- get '/restaurants/:id' : Shows information from one restaurant entry by ID
- get '/restaurants/new' : Shows page to enter information for new restaurant entry
- post '/restaurants' : Provides functionality to CREATE new restaurant entry
- get '/restaurants/:id/edit' : Shows page to UPDATE information for one restaurant entry by ID
- put '/restaurants/:id' : Provides functionality to UPDATE information for one restaurant entry by ID
- delete '/restaurants/:id' : Deletes record of one restaurant entry by ID

17. What's a migration?

Instructions on how to create database.

18. When you create a migration, does it automatically modify your database?

I don't think so.. within your seed file, you can specify columns to delete, etc.

19. How does a model relate to a database?

Models interact with the database. There are inherited ActiveRecord methods to search for instances of models within databases.
- Every controller has access to every model in the database.

20. What is the difference between `#new` and `#create`?

New makes an instance of the model but does NOT automatically save it to the database.
Create automatically saves a new entry to the database.
