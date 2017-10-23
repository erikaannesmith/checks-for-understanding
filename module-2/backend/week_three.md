## Week Three Recap

### Instructions
Fork this repository. Be sure to pull the latest changes to your local repo. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Questions

1. What is the entry at the command line to create a new rails app?

rails g new app_name [-T -d="postgresql" --skip-spring --skip-turbolinks]** this part is optional

2. What do Models generally inherit from in rails?

ApplicationRecord

3. What do Controllers generally inherit from in a rails project?

ApplicationController

4. How would I create a route if I wanted to see a specific horse in my routes file assuming I'm sticking to standard conventions and that I didn't want other CRUD functionality?

in config > routes:
resources :horses, only: [:show]

5. What rake task is useful when looking at routes, and what information does it give you?

rails routes
it allows you to see the prefix, verb, URI, and action#path of all routes that have been configured

6. What is an example of a route helper? When would you use them?

I think an example of a route helper could be a link_to. You would use them inside view pages to, when executed, send users to the specified route.

7. What's the difference between what `_url` and `_path` return when combined with a routes prefix?

`_url` generates a string with an entire URL and `_path` generates the relative path from the root of the app.

8. What are strong params and why are the necessary?
9. What role does `form_for` play in helping us create our forms?

Form for creates a form for whatever you pass in through the instance variable.
Depending on the route specified in the controller, it will create a new instance, edit an existing, etc.

10. How does `form_for` know where to submit the user's input?

From the instance variable in the first line

11. Create a form using a `form_for` helper to create a new `Horse`.

<%= form_for @horse do |f| %>
 <%= f.label :name %>
 <%= f.text :name %>
 <%= f.submit %>
<% end %>

12. Why do we want to validate our models?

To ensure that they have all necessary attributes when they are being created.
