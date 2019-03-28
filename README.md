# JavaScript assignment

## Some useful resources
* Some [JavaScript tutorials](https://www.htmldog.com/guides/javascript/)
* The complicated [resources in the You Don't Know JS](https://github.com/getify/You-Dont-Know-JS) series, including [your reading last week](https://github.com/getify/You-Dont-Know-JS/blob/master/up%20%26%20going/ch2.md)
* [A resource for CSS/style/colors](https://htmlcolorcodes.com/)  
* [An excerpt from a specific workshop site](https://witny-summer-guild-2018.github.io/day_4_exercise_2.html) (for a different audience than yourselves) which addresses some common questions about jQuery
* [The simple JSFiddle example from class](https://jsfiddle.net/2of65j8q/)
* A [W3Schools resource on JavaScript output](https://www.w3schools.com/js/js_output.asp)
* Google, Piazza, your classmates, office hours, lab time!

## Included files
* This `README.md`, which you should edit with answers to the questions
* `jsPracticeLab.html`, which you'll need to edit and try out
* `jquerylib_submit_example.html`, which you'll need to edit and try out

## Your goals for this lab

### Broadly
The aim for this lab is to practice adapting to and understanding code in a new-to-you (or not) language and its own libraries/packages -- JavaScript, in this case.

The programming skills you have built up till now are useful for *Python programming*, but, more than that, they extend to fundamentals of many kinds of programming.

This experience is *not in any way* about becoming an expert JavaScript programmer. Instead, it is about using what you *do* have experience with -- and your skills in *learning new things* that relate to programming -- in order to make educated judgments about some brand new-to-you code, even if you haven't learned in detail about it yet. That's part of what being in technology -- or even technology-adjacent -- will often mean.

### Specifically

Below are a bunch of questions and indications of things to do. For each indication of something to do with code, there is also an accompanying question to answer or brief explanation to give.

**To complete and submit this assignment, you should:**

* Fork (and clone) this repository
* Add our instructional team as a collaborator to your fork (see instructions for adding collaborators on Canvas)
* Edit this `README.md` file with answers to the questions/prompts, briefly, using Markdown formatting so that the questions appear in bulletpoints and the answers appear clearly below each respective question, *not* as bulletpoints.
* Add all names of those who worked on this (as indicated below)
* Make the changes that are indicated below to each of the `.html` files with JavaScript programs provided. (You'll probably do this concurrently with answering questions)
* Commit (as you go) and push your changes to all three files to your GitHub forked repository.
* Submit a link to your repository on Canvas. (This HW doesn't have an autograder -- it will be graded by hand/by humans this time.)

### Important notes
* You are *more than* welcome to work together on this, but **you must <u>each</u> submit a repo to be graded on it**, so if you do work together, you should do the following:
	* Make sure each one of you understands all the work -- YOU are responsible for using and knowing this information
	* Write each person's name & uniqname who worked on the assignment together on your submitted `README.md` file (you'll see a space for this below)

* In answering questions, please make sure the formatting is clear to read and that you have updated the names of everyone who worked with you, with your name first (see below).

* In answering questions, assume all of the questions include a *explain briefly* note -- you do NOT have to, and should not, write extended paragraphs. Be as concise as you can and explain in your own words. Don't worry about "whether it's enough" -- just worry about conveying your understanding so you can read it later, or even give it to someone else, and the answers will help/make sense.

* It is not acceptable to copy and paste answers from the internet and submit them as your own. If you cite things, make sure you provide a citation, including to links. If you get information from a resource and rephrase it so you're basically explaining an idea, that's just fine for an explanatory purpose in this assignment, but you *must* cite any quotes or examples that aren't yours.

* **For grading:** we are grading on...
	* Following the instructions
	* Approximate correctness of the code edits
	* Careful & clear answers to the questions
	* Correct answers to the questions
	* Slightly more than half the 1000 points will come from answering the questions. The rest will come from your edits to the code.

### Names of people you have worked with on this assignment
* List everyone's names and uniqnames who have worked on this assignment with you, **including your own name, but make sure YOUR name is first and bold**
* Like this:
* **Amanda Jung (amajung)**

## Questions & code instructions

### The first questions address the `jsPracticeLab.html` file.

* **This is just an example question.**

This is what an example answer should look like. If you want to include some code, which you probably don't have to do, you can, like this:

```js
Some JavaScript code
```

* **What does a code comment look like in JavaScript? What character/s do you have to put before a comment?**
A code comment looks like the following:

```js
// This is a one line comment.

/* This
is
a
multi-line
comment.
*/
```
The characters you use for a one line comment is this character ```js // ``` while the the characters you use for a multi-line comment begin with ```js /* ``` and ends with ```js */ ```.

* **Explain what needs to happen to get a JavaScript program to "run", given the JavaScript you've seen in this assignment.**
In order for a JavaScript program to "run", the user must link their Javascript code to or include it within their HTML file when they run it.

* **What functions in JavaScript seem to be similar in function to the `print` function in Python? (There are two.) Why might you use one and not the other? Explain briefly.**
The two functions in JavaScript that seem to be similar in function to the `print` function in Python are the `alert()` and `console.log()` functions. The alert() function displays text in a pop-up box and would be best when getting a user's attention. On the other hand, the function console.log() outputs messages to the console and would be best used for debugging or testing purposes.

* **What code would have to comment out to get rid of the pop-up box when you load the page? (Related to the last question.) Do that in the code file, and then, add code so that a text box will appear that contains the current date and time! *HINT:* Look through the rest of the code first...**
The code that would have to be commented out to get rid of the pop-up box when you load the page is `alert("hello");`. To make a text box appear that contains the current date and time, you would add the line `alert(new Date());`.

* **How can you put your own name at the top where it currently says "A name"? Explain very briefly how to do so, and replace `A name` in the web page with your own name.**
You can put your own name at the top where it currently says "A name" with the following line of code: `document.querySelector('h1').innerHTML = "Amanda";`. The code essentially changes the content of the HTML element, which in this case is the h1 element.

* **What does the word `document` represent in this code? Explain briefly.**
The word `document` represents the whole HTML document that's displayed in the window. It is usually the precursor to accessing any element in an HTML page. For example. to find an element by Id you would use the method `document.getElementbyId(id)` or to find an element by Class `document.getElementbyClass(name)`.

* **What is happening in line 12 (
		`document.querySelector('#items').innerHTML = document.getElementsByTagName('li').length`
)? Explain, briefly (<= 2 sentences).**
Based on the code in line 12, the code on the right side of the equal sign (`document.getElementsByTagName('li').length `) obtains the number of list item tags (`<li>`) while the code the left side of the equal sign (`document.querySelector('#items').innerHTML`) accesses the HTML span element and its content with its id `items`. Altogether, the code on line 12 finds the number of list items tags, assigns it to the HTML element of id `items`, and displays it.

* **What color would the background of this page be <u>if there were no JavaScript in this page</u>?**
The color of the background of this page would be white (#ffffff) if there was no Javascript.

* **Why are there a couple of gray boxes on the screen with a different colored border? How could you edit this code to make them a different color? Explain briefly. Then edit the code to make those boxes some shade of blue, of your choosing.**
There are a couple of gray boxes on the screen with a different colored border because of the HTMl and CSS code that's written in the file. To make them a different color, you would edit the CSS code by changing the background-color and/or border attribute to the desired color.

* **Edit the code so that, if you highlight `McGill University` and copy it, you see the text `O Canada` near the bottom of the page. Briefly explain why you made the edits that you did -- how did you know/figure out what to do?**
I knew/figured out what to do by observing the function of `copyFunction()` and the way it was linked to the text `University of Michigan`. I then copied `copyFunction()`'s code, changed the copied function's name to `copyMcGill()`, and altered its text to print `O Canada`. To make sure the function was implemented correctly, I linked it to the text `McGill University` by assigning `copyMcGill()` to the `onCopy` event.

* **In the original code, when you click the button that says `Wow`, you see a text box! Wow. Explain briefly in your own words why the following code causes that to happen:**
```js
function handleClick(){
	alert("hello");
}
```
**and**

```js
<button onclick=handleClick() id="wow-button">Wow</button>
```
The HTML and Javascript code above causes a text box to appear when the user clicks on the button that says "Wow". For example, the first chunk of code (Javascript) defines the function `handleClick`. When the line ```alert("hello");``` runs inside the function, a pop-up box with the text `hello` will appear. Not only does the second chunk of code (HTML & Javascript) create the button and its text `Wow`, it also links it to the Javascript function `handleClick` with the code `onclick=handleClick()` and causes it to run. Altogether, the second chunk of code (HTML) will run first then the first chunk of code (Javascript).

* **Knowing what you learned from the previous question, add code/markup to the `jsPracticeLab.html` file *so that* there is a button with the text `Spring Equinox 2019` on it somewhere on the page, and when that button is clicked, a text box containing the text `March 20, 2019` appears. (There's no function -- that I am aware of -- to automatically get this info, you've got to type it yourself.)**
The code below showcases the instructions above:

```js
function SpringEquinox(){
	alert("March 20, 2019");
}
```
and

```js
<button onclick=SpringEquinox() id="se-button">Spring Equinox 2019</button>
```


### The next few questions address the `jquerylib_submit_example.html` file.

* **Check out the file `jquerylib_submit_example.html`. This is an example of code that uses a package called `jQuery` (and this will need you to have an internet connection to run it properly, although the other file does not). Check out resources above for more on jQuery!**

* **When you enter input that isn't valid, you see an error that is red. Why is the error in red? Why is the response for valid inputs blue?**
The error is in red because the class that the text is contained in is styled to be red using the CSS color property. The response for valid inputs is blue because the text is contained in is styled to be blue using the CSS color property.

* **What is this line `var regex = /^[a-zA-Z]+$/;` helping with? And if you googled something to figure that out, what did you google, and what, briefly, did you learn? (If you didn't need to google, you can leave that out, but explain briefly what that line is helping the program do, anyway.)**
The line `var regex = /^[a-zA-Z]+$/;` helps with testing to see if the text that's entered contains only characters a-z or A-Z. To figure this out, I googled `var regex = /^[a-zA-Z]+$/;` and learned that it is a regular expression for only characters a-z and A-Z.

* **What's different about the syntax of conditional statements in JavaScript, compared to Python?**
The syntax of conditional statements in JavaScript include parentheses around the boolean expression and brackets surrounding the code that's to be executed if the boolean expression is true. On the other hand, the syntax of conditional statements in Python does not and only has a colon prior to to

* **What do you think the `10000` refers to in the code `.fadeOut(10000)`?**
The `10000` in the code `.fadeOut(10000)` refers to the message that's linked to it fades out after 10000 milliseconds (or 10 seconds).

* **What do you think is going on with the following code at the beginning of the program? Note that the most important thing to do for answering this question is to be thoughtful and clear, not to be absolutely correct:**

```js
$(document).ready(function(){
    $("form").submit(function(event){
```

Based on what I searched on Google, the line `$(document).ready(function(){.` will indicate whether the code below it will run once the the Document Object Model (DOM) becomes safe to manipulate or is `ready`. On the other hand, the line `$("form").submit(function(event){` triggers the submit event for the form leading the function within it to run.

* **Add some code to the `jquerylib_submit_example.html` file so that, if the input is valid and is specifically the text `hello`, rather than the visible output being `Nice!` in blue, the visible output should be `Hello to you too!`, also in blue, just like `Nice!` is.**
* *HINT:* You'll have to make some changes to the conditional statement, and possibly look up some JavaScript conditional syntax. You'll also need to look carefully at what generates visible output right now.
