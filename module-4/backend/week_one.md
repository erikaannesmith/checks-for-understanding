## Week One - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. What's the most useful thing you learned from completing the intermission week work?
For me, I try to take the intermission work as initial exposure to whatever concepts we'll be learning during the mod. I try to digest the material as muscle memory and syntax exposure.
2. What are some tools to help debug JavaScript code?
DevTools, debugger, pryjs, console.log
3. What are some tools you need in order to unit test your JavaScript?
mocha
4. What is the syntax for invoking a function?
function x( , {

})
OR
const x = () => {

}
5. What's `this` in JavaScript?
this is whatever it is being called by. meta...
6. What is Webpack and why is it useful?
webpack is the compiler for javascript, kind of like the asset pipeline.
7. When/why do you want to use event delegation?
it allows you to use a single event listener, but interact with it on multiple layers.
8. What's `npm` and what do we use it for?
node package manager, it is how we start our server, install packages, etc.

#### Review  
9. What's the MVC design pattern? Describe each part of MVC.
model, view, controller. model is the class of the objects, which instances will be made of. it includes attributes and any methods that are specific to that object. 
instances of the model are created/instantiated in the controller and passed through to the view.
the view is what will be rendered to the client, and usually references the instances created in the controller.
10. What are a few ways to optimize a Rails application?
redis/sidekick
11. What's a background worker? When would we want to use a background worker?
a background worker is something that allows your app to continue a process in the background without holding up the app's next move. we would want to use one if the task is something that doesn't need to be completed immediately.
