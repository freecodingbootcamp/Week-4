# Week-4 -- Day-1

## Intro to JavaScript

###  JavaScript as a Language

JavaScript is a programming language. Just like with human languages, it comes with its own set of rules and grammar. And just like with human languages there can be some overlapping with other programming languages. Also, Java and JavaScript are not the same. While JavaScript is evolving to be more like Java it is still not Java. Do not use them interchangeably.

JavaScript started off being a front-end language but can now be used on the backend as well.
A front end language is just a language that runs within the browser. As in it does not run on a server thousands of miles away but instead runs on your very own computer every time you load a web page!

### JavaScript Frameworks?

Web frameworks are just a pre-configured system that consists of a bunch of libraries/tools that work together to make web development easier and more effective. You can do more with less if you will. At least that is the idea.

Here is another definition by GeeksforGeeks:

> _a software framework that is designed to support the development of web applications including web services, web resources, and web APIs_

I'll leave it up to construct your understanding of a web framework.

Back to JavaScript...here is a shortlist of the most popular JavaScript frameworks:

 1. Angular (by Google)
 2. React (by Facebook)
 3. Vue
 4. Node (Server-Side/Backend)

My favorite is react + node, mainly because that is what I started off learning first and got better at. It might also be one of the most popular web framework combos out there.

### Where to Write and Run JavaScript Code

#### 1) Browser Console
You can use the console within the dev tools to write and run JavaScript. It's a great place to run something real quick but definitely to run anything significant or longer than one line of code!

#### 2) Repl.it

You can also use an online editor + compiler such as repl.it

#### 3) Using Script Tags in HTML

Finally, the most common way to use and run front-end JavaScript is withing script tags in HTML. You can either link to an external .js file or just put all JavaScript within a script tag.

    <script>
	    console.log("Hi from within script tags!");
    </script>

or link to an external file

    <script src="js/script.js" charset="utf-8"></script>

In the case above we assume there is a folder called 'js' and file 'script.js' inside of it.

I recommend you put/load any JavaScript towards the end of your HTML page so probably right before you close your body tag.

## Let's Code in JavaScript

### Printing out to the screen
Sometimes you just need to print something out so you can see it's value. You can use console log for that! So:

    console.log("Message here!");

 This will print something to the console. In this case, it will print "Message here!" without the quotes.

### Comments

To comment a line of code so it does not get executed you can use:

    // console.log("This does not get printed!");

or for multiple lines use /* */ so

    /*
    console.log("This does not get executed!");
    console.log("Why am I using so many exclamation points!");
    console.log("Oh man I did it again! Why can't I stop!");
    */

### Variables

Sometimes you need to store a value like a number and give it a name so you reference it later. Here is how you can do so:

    let myAge = 113;

so every time I call on myAge without quotes it will be replaced by 113.

Simple right? And look no exclamation point! Oh noo...

### Strings, Booleans, and Numbers

There are different types of data types in JavaScript. We are going to focus on three of the primitive types here.

#### Strings

Strings are text or words. What I am writing right now would be considered a string. Albeit a very long one but a String none the less. Strings are usually wrapped around quotes so either single or double-quotes.

    'I am a string'
    "So am I"

#### Booleans

Booleans are the most computer concept I can imagine. It's literally either true or false and that's it. So here is an example of declaring and initializing a boolean that is set to whether I am currently fasting or not:

    let isFasting = false;

So if I do a `console.log(isFasting);` it should print out `false`

#### Numbers

Numbers like the name suggest represents a number. So you can do mathematical operations on them. You can add them, divide them, etc. Something like this:

    let result = 4 + 6;

Here 4, 6, and result are all numbers. Simple right?

### Arrays

What if you want to store multiple numbers but only use one name? Easy peasy we can use Arrays. So let's say you want to store student grades into a variable called...grades.

    let grades = [99, 80, 97, 67, 100, 100, 70];

Easy right? So how do you access an individual grade? Here is how you can access the second grade.

    console.log(grades[1]);

Notice I used 1, not 2 to access the grade. That is because arrays start at 0, not 1.

### Functions

Functions are a fundamental part of programming. Functions are the verbs of a programming language. They represent an action. So let's create a function that takes in two values and returns the sum of them.

    function addTwoNumbers(a, b) {
	    return a + b;
    }

function is a keyword followed by the name of the function then the parenthesis that holds any arguments the function might need followed by the curly brackets that contain the actual body of the function.

Please distinguish between defining a function and executing/calling a function. The function does not run until you call on it. Here is how we can on the function above with two values for a and b.

    addTwoNumbers(3,4);

The function call above returns 7. You can do whatever you like with this value. So let's just store it.

    let result = addTwoNumbers(3,4);

Now the result holds the value of 7.

Easy right?


### Continue on W3 Schools

Please please please go through all the W3 schools javascript tutorial.

Here is the link: https://www.w3schools.com/js/default.asp

Start at JS HOME and finish with JS JSON

W3 Schools uses js element selectors a lot. I personally would not have used element selectors to demonstrate vanilla javascript but hey I am not W3 schools. Also, keep in mind W3 schools uses var instead of let. I would highly recommend you use let not var.

Oh, I almost forgot! We also have constants. Constants are variables that you cannot change.
So if you wanted to declare a constant you would do the following:

    const b = 34;

Now you cannot change the value of b.

OK, I think that was it in terms of a super basic intro to JavaScript.
