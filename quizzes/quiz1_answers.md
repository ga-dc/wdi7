# Quiz #1 - Answer Key

## Question #1

**Which of the following terminal commands demonstrate correct syntax?**

**Correct Answers:**

* `mv main.css ../css/`
* `mv -n main.css css/`

**Incorrect Answers**

* `mv main.css css/ –n`
  * This is incorrect because you can't put an option after the arguments
* `mv ––n main.css css/`
  * This is incorrect because options with 2 dashes take the form of a whole word, not a single letter

## Question #2

![](https://lh4.googleusercontent.com/k3E-Ro9MazYsV_Kw_BMMCDAOsrK93sg6Ls_Jxo1YUCqZgqhVRNCOOQW7Zh-3FX39y7FIFA)

**You are currently in the "code" folder. How would you get to the folder that contains "beach.png" using the command line? **

**Correct answer**

`cd ../../photos/summer_vacation_2014/`

Note that the final `/` is optional, and we gave credit if you omitted the `cd` command, or included the file beach.png.

However it's important to note that you can only `cd` into a **folder**, so if you included **both** the `cd` and the file name, that command wouldn't work.

## Question #3

**What is specificity? How is it related to class and id selectors? **

**Correct Answer**

`Specificity determines which styles are applied to an element. More specific rules take precedence. IDs are more specific than classes.`

All other answers are incorrect.

## Question #4

**What are the components of the box model and what do we use it for? **

**Sample Correct Answer**

```
In CSS, each element is a rectangular box. The box model describes the parts of each box, and how they relate to the total size of the box.

There are four main parts:
* Content area - this is the inner most area where content such as text, images, or other HTML elements are displayed.
* Padding - space between the content and the border
* Border - this may be invisible or have a width and color, pattern, etc. When it has a width, it's the visible edge of the element.
* Margin - this is space outside the border that separates one element from other elements near it.
```

## Question #5

**Why is it important to keep semantics (HTML) separate from style (CSS)? (CHOOSE ALL THAT APPLY) **

**Correct Answers**
* It makes our HTML/CSS more readable.
  * Removing style from our HTML makes it more concise and focused on the content and structure, which improves readability.
* It makes it easier to update our HTML/CSS as we need to make changes
  * By separating our Content/Style, we can add new content without having to re-define styles, and we can change styles without having to modify the content.

**Incorrect Answer**
* It allows the browser to make fewer requests to display a page.
  * Separating CSS into a separate file forces the browser to make an additional request(s) to download the CSS file(s). However, this cost is very small compared to the benefits we get from separating HTML/CSS
* It's not. Advanced developers often mix them together for an improve user experience.
  * There are no features / user experiences that require in-line stylesheets to function.

## Question #6

**Which of the following represents a common git workflow? **

**Correct Answer**

* `git add file_name; git commit -m "my message"; git push origin master;`

**Incorrect Answers**

* `git commit file_name; git add -m "my message"; git reset; git push origin master;`
  * `git reset` will undo our `git add` command. Also, `git commit` can't come first.
* `git add file_name; git commit -m "my message"; git push origin master; git reset;`
  * there is no need to `git reset` after a `git push`
* `git add file_name; git commit -m "my message"; git pull origin master;`
  * performing a `git pull` will not share our changes with others, we need to `git push`  
* `git stage file_name; git commit -m "my message"; git push origin master;`
  * there is no `git stage` command. The correct command is `git add`

## Question #7

**What is the difference between a fork and a clone?**

**Sample Correct Answer**

```
A fork is when you make a copy of a repo on GitHub. The copy is associated with
your account, and thus you have full control of the forked repo, including
pushing changes. (You may or may not have permissions to push changes to the
original repo that you forked.)

A clone is when you use git to download an entire repository (and all it's
history) onto your own computer. When cloning a repository, it's linked to the
one you cloned, so you can use git push/pull to share/retrieve changes, assuming
you have permissions.
```

## Question #8

**Write a JS function called `add` that takes two arguments, adds them together, and returns the result. **

**Sample Correct Answer**

```js
function add(number1, number2) {
  return number1 + number2;
}

// or you could store the function in a variable (expression vs declaration)

var add = function (number1, number2) {
  return number1 + number2;
}

// or you could store the sum in a variable returning it

function add(number1, number2) {
  var sum = number1 + number2
  return sum;
}
```

Note that there are other correct answers, but we were looking for something
along these lines.

## Question #9

![](https://lh3.googleusercontent.com/3RM0-dKy82N5yBPgSYHcVdC6rRg7peYYEexMA66Fydyj57Ij6GYMabj6mU-ka2qqcUh0Ww)

**Which of the following is a valid way to get the model of the `car` object?**

**Correct Answers**

* `car.model`
* `car["model"]`

**Incorrect Answers**

* `car[model]`
  * when using the square bracket notation, we have to put the property name as a string
* `car."model"`
  * when using the 'dot' notation, you can't put the name of the property in quotes
* `car.get("model")`
  * there is no `get` method in plain JS
* `fetchProperty("model", car)`
  * there is no fetchProperty function in plain JS
