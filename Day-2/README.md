# Week-4 -- Day-2

## Intro to JavaScript Continued

### Conditional Statements

#### if statement

Sometimes you want to run code but only if something is true. So let's say you want to display a message that says "Welcome Back" if somebody is logged in. So you would do something like this:

    let isLoggedIn = true;
    if(isLoggedIn){
	    alert("Welcome Back");
    }

Simple right?

Make sure you have a statement that evaluates to true or false inside the if parenthesis ().
So the simplest version of that is either `true` or `false` so

    if(true){
    	// Do something here
    }

But you can also have something a little more complex. Something like

    let rewards = 1230;
    if(rewards > 1000) {
    	// Their coffee order is free
    }

Here `rewards > 1000` evaluates either to true of false assuming it doesn't trigger an error message.

#### Adding an else statement

Sometimes you need one of two things depending on if something is true or not. So using the rewards model again we could do something like this

    let rewards = 1230;
    if(rewards > 1000) {
    	// Their coffee order is free
    } else {
	    // Display a message stating they don't have enough points
    }

So **ONLY ONE** of the two statements above will execute but **NOT BOTH**  unless something triggered an error of course.

Not too bad, right?

#### Multiple conditions

What if two things have to be true in order for something to run. So let's say in addition to having enough points they cannot have ordered a free coffee today already.

    let rewards = 1230;
    let eligible = true;
    if(rewards > 1000 && eligible) {
    	// Their coffee order is free
    } else {
	    // Display a message stating they are not eligible
    }

Notice the two ampersands (&&)? That means both conditions have to be true in order for the first statement to run. If one of the two statements is false the else block gets run.

### Converting Between Types

Remember how there are 8 types in JavaScript and we on three (Boolean, Number, String) of them? Well, guess what you can convert amongst them! So you can turn a Number into a String.

![Snoop Dog morphing into a well...dog](https://media.giphy.com/media/3otPoOrOg3KTKs9AJi/giphy.gif)

Here is how you can convert a Number to a String

    let num = 10;
    let str = num.toString();

str is a string that looks like this "10" instead of like this 10. Notice the quotes.
`toString()` is a built-in function that you can call on any Number variable.

How do you convert a String to a Number.

Easy, you use a function called `parseInt()` but you don't call it on a string variable. Let me just show you an example:

    let str = "22";
    let num = parseInt(str);

Now num should be 22 not "22".  Notice how in `toString()` you use the variable name then the .toString() while in  `parseInt()` you provide the string as an argument within the parenthesis. Don't worry about the why part just yet. Just be aware of the difference. 
