# Quiz #1 - Answer Key

## CSS

### Question

Describe the purpose of a clearfix in CSS, and give an example of how to do it.

### Question

What does the following selector do?  `ul.dropdown > li`

```
* Selects all li's which are directly inside a ul of class dropdown (children)
* Selects all li's which are anywhere inside a ul of class dropdown (any ancestor)
* Selects all ul's of class dropdown, as well as the children elements that are li's
* Selects all ul's of class dropdown, only if their children are exclusively li's
```

## Scope/Context/Closures

### Question

Describe the rules of scope in JavaScript.

### Question

Define an object and store it in a variable `pizza`. The object should have 2
properties: a temperature (set to 70), and a method called `bake`. When called,
this method should set the pizza's temperature to be 300. Note: you may not use
the variable pizza inside your method.

## Callbacks

### Question

**Define a function called `doSomething`. It should take one argument, called
`thingToDo`. When called, thing to do should invoke the function given as an
argument. Finally, demonstrate calling `doSomething` with a function.**

### Question

**What is the difference between synchronous and asynchronous program execution?**

```
* Synchronous code runs at an even pace, asynchronous code runs with uneven pacing.
* Synchronous code runs all at the same time, asynchronous code runs completely randomly
* Synchronous code runs in order (as appears in the source), asynchronous code may run at a later time.
```

## Git

### Question

Which of the following represents a correct workflow for submitting a PR on a non-master branch?
(ignore the lack of commit messages)

```
* fork on github; git clone <fork_url>; git checkout -b <charlie_solution>; git add <files>; git commit; git push; create pull request
* fork on github; git clone <ga_dc_url>; git checkout -b <charlie_solution>; git add <files>; git commit; git push; create pull request
* git clone <ga_dc_url>; git branch <charlie_solution>; git add <files>; git commit; git push; create pull request
* fork on github; git clone <fork_url>; git checkout -b <charlie_solution>; git add <files>; git commit; git pull; create pull request
```

## jQuery

### Question

Which of the following statements will work, assuming jQuery is loaded? SELECT ALL THAT APPLY

```
* `$(".post").css("background", "peachpuff")`
* `$(".post").innerHTML`
* `$(".post").html()`
* `document.getElementsByClassName("post")[0].innerHTML`
* `document.getElementsByClassName("post").innerHTML`
```

### Question

Using jQuery, add an event listener for clicks on the button with the id
'greeting'. When the event happens, the code should append a paragraph to the
body, that says "hello".

## Software Development Processes

### Question

Write out three (3) user stories for your first project. Be sure to include a
role, goal, and reason for each.
