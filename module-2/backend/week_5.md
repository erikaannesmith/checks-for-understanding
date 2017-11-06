1. How do we make flash messages display on a page?

use an each block within the application.html page to show how to display the information(it's stored as a hash) and put somthing along the lines of:
flash[:notice] = "Successfully created an object"
in the controller to signal that an object has been altered.

2. Where is cart information/temporary information usually stored?

session

3. What might be some reasons not to store cart in our database? Are there any reasons why we would want to persist that information?

it would take up a lot of space and is altered frequently.. it would be a lot of back and forth to the database. storing it in a session keeps the information at surface level until the order is placed.

4. What is the purpose of the asset pipeline?

the asset pipeline is responsible for compressing and preparing assets to serve to the browser.

5. Why do we precompile our assets?

because the browser doesn't receive our code the way we write it- we write it in a more developer-friendly way that's then precompiled and translated from multiple languages into what the browser receives.

6. What do each of the following tags do?

```ruby 
<%= stylesheet_link_tag "application" %>
<%= javascript_include_tag "application" %>
<%= image_tag "rails.png" %> 
```
each links assets to the asset pipeline (stylesheets, js files, and images, respectively)

7. What are some of the elements of a great read me? What are some of the benefits of taking the time to update a readme for our project?

a great readme should include any setup required for the app, current rails version, etc. it should also have the purpose of the app and any errors that are common with solutions. having a great readme makes your app more accessible to all users and increases the likelihood that it will be shared.

8. What are the top four accessibility issues that we as developers should be aware of?

cognitive, visual, mobility, hearing

9. `before_save` is an example of a what? Where in our Rails application would we find a `before_save`?

it's an example of a callback and we might find it in the create method of a controller

10. Given the following object, how would we create a scope for all users who are active?

```ruby 
User.create(name: "Happy", active: true)
```

scope :user, where( active.true? )

11. What is the difference between a scope and a class method?

scope methods are used to define the range within to look for something. for example: 
scope :word, where( split.count == 4 )