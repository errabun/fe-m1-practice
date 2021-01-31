***Chapter 3 - Functions and Scope***

1. If we have a function defined as function sayHello(){console.log("Hello!")}, what is the difference between entering sayHello and sayHello() in the console?

  - If we just enter sayHello into the console, it will return the entire function.  Whereas if we enter sayHello() to the console, it will log Hello! in the console.  Using the parentheses actually fires the function, in this case the only statement to be executed is to log Hello! to the console.  


2. What is the difference between function parameters and arguments?

  - Parameters are act like variables in a function declaration.  They are pieces of information that we can add to a function declaration in order to get a desired result from a function declaration.  When we call the function in code, we use arguments as those variables in the call to the function.  
    ```javascript
    var greeting = function(name) {
      console.log("Hi " + name + "!");
    }

    greeting("Eric");
    ```
    In the example above, we are saving a function in a variable named greeting.  The function is going to take one *parameter* which is a name.  When we call the greeting function later in code we use an *argument*, in this case "Eric" to log Hi Eric! to the console.


3. What is the keyword return used for?

  - When you would like a function to return a single value, you would use the keyword return at the end of the function declaration to tell interpreter to return that value.  
  ```javascript
  function calculateArea(width, height) {
    var area = width * height;
    return area;
  }

    var wall = calculateArea( 4, 9);
  ```

  In this example we create a function named calculateArea with two parameters, width and height.  In the function we create a variable named area and assign the value to be the width times the height.  Seeing as we are seeking the value from our area variable, we use the return keyword on our variable area.  So, when we call the calculateArea function and pass 4 (width) and 9 (height) as arguments, our function will return the area of a wall 4' x 9'.

4. How are local variables better than global variables? Are there instances you can think of where you might want to use a variable that is globally scoped over local?

  - Local variables are better than global variables in a script because when loading a page, the interpreter has to save all global variables in memory for as long as page is loaded.  As well, you may run into some naming conflicts if you are using lots of global variables.  Local variables are created inside a function and cannot be accessed outside the function in which it is declared.  
    One instance where you may want to use a globally scoped variable would be for a piece of information that is not going to change anywhere in the script, such as a name or username.  Say you wanted to have a greeting when someone logs into your page.  The name you would use for the greeting is never going to change.  Also say they are going to purchase something and you need their shipping information.  You could use their name/username to automatically fill in some of the shipping information for them.  
