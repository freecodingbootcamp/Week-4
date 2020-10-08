# Week-4 -- Day-3

## JavaScript Continued

### Arrays
So you want to store more than one value reference it using a variable. What is the solution?
An array!

> ... the **word array comes from** the Old French areyer, "to put
> in order,"

That is what we are doing when we are storing elements in an array. We are putting them in order. They are not just thrown into a collection without any order. Let me just show you:

    let arr = ["Hamilton", "Ricardo", "Vettel", "Verstappen"];

 Here we have a variable called arr that stores 4 names. The first name that is being stored in "Hamilton". What if I wanted to console.log that first name? Easy!

    console.log(arr[0]);

**arr[0]** retrieves the value of the first element in the array. Remember **arr** is just the name of the array. It's a variable name. It can be anything you choose as long it's OK with JavaScript.

You might be wondering how do I add an element? Easy. Arrays come with built-in functions. Don't worry if the built-in function part confuses you. But back to adding an element to the array. Let's say we want to add "Albon" to the list. Here is how you would do it.

    arr.push("Albon");

Can you guess where in the array "Albon" would fall into? The end. That is correct.

So the array now looks like this:

    ["Hamilton", "Ricardo", "Vettel", "Verstappen", "Albon"]

What if you wanted to change the value of an element? Again, easy peasy. Let's say we wanted to change "Hamilton" to "Bottas". Here is how you would do it.

    arr[0] = "Bottas";

The array that we called **arr** now looks like this:

    ["Bottas", "Ricardo", "Vettel", "Verstappen", "Albon"]

How about printing or console logging every single element?

You can use a loop for that. But before we go into for-loops I just wanted to show you an array of attribute that might be useful. The attribute is .length so if you call to do `arr.length` it will return how many items are stored in the array. So `arr.length` will return 5.

### For-Loops

Loops are as the name suggests...loops. You tell it how many times to loop and it will loop that many times. So let's say you want to console log the numbers ranging from 1 to 10. So start at 1 and end at 10. There are many different types of looks but I am just going to go over one of them: for-loop. So here is how you would do it in a for-loop.

    for(let i = 1; i <= 10; i++){
    	console.log(i);
    }

This will console log 1 2 3 4 5 6 7 8  9 10 each number on its own line.

Here is a syntax breakdown of a for-loop

for(where to start; where to stop; what to do after each iteration) {
	// Body of code to run each iteration
}

so let i = 1 is saying run this when you start the for-loop, i <= 10 is saying keep looping as long as i is less than or equal to 10 and finally increase i by 1 after each iteration.

Here is the equivalent while loop version:

    let i = 1; // Where to start
    while(i <= 10){ // When to stop
	    console.log(i);
	    i++; // What to do after each iteration
    }

So let's look at how you can use for-loops to console log each value of an array. So let's say the array is arr again. So to refresh your memory this is how we initially declared and initialized it:

    let arr = ["Hamilton", "Ricardo", "Vettel", "Verstappen"];

Here is the for-loop to print out each value:

    for(let i = 0; i <= arr.length; i++){
        	console.log(arr[i]);
        }
That's it.

### Strings

Strings are text. They are just words, characters. They are used for the value part of a variable.
So let's say you wanted to store your name in a variable called name. You would do the following:

    let name = "Erika";

The double quotes are the defining characteristics of a string.

Let's say we have two strings

    let title = "Nurse";
    let name = "Erika";

We can console log those two together and maybe even add some more custom text to it.
So let's console log **"Erika is a Nurse"** but using the variables above. Here is one way it can be accomplished.

    console.log(name + " is a " + title);

This is called string concatenation.

Another interesting thing about strings is they behave like arrays where each element in the array is a character of the string.

So in the variable name I can access the second character **"r"** by doing what we would do in an array, `name[1]` so to print the first character along with the last character you could do:

    console.log(name[0] + name[4]);

You could also retrieve the total number of characters in the string by using the length attribute.

    console.log(name.length);
