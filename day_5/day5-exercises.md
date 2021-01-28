***JavaScript & jQuery - Chapter 2***

1. How do you declare a variable. What does the equals sign really mean in JavaScript? What is it called in JavaScript?

  - A variable is declared by using the variable declaration keyword var (const or let) followed by a variable name.  There are specific rules for naming a variable (see below).  The variable name is followed by an assignment operator (=) and a value assigned to the variable name.  The equals sign really is an assignment operator in JavaScript.  It assigns the value to the right of the equals to the variable name (to the left of the equals sign).


2. There are three big data types in JavaScript: numbers, strings, and booleans. Describe what each of them are.

  - Numbers are a numeric data type and can be any type of number; positive, negative or a float (decimal number).  They use no commas in JavaScript.  
      ex: var age = 33;  
  - Strings data type are made up of letters and other characters and are enclosed in a pair of quotes (single or double).  Use when working with text in JavaScript.
      ex: var firstName = 'Eric';
  - Booleans are a data type that have one of two values -> true or false.  
      ex: var isRaining = false;


3. What are the six rules for naming variables? What are a few JavaScript reserved words that you should avoid using for variable names?

  - The six rules for naming variables are as follows:
    - Variable name must begin with a letter or underscore
    - Name can contain letters, numbers, dollar sign ($), or an underscore (_); no dashes or periods in a variable name
    - Cannot use any JavaScript keywords; such as naming a variable var
    - Names are case sensitive.  So greeting and Greeting are two different names in JavaScript
    - The name should reflect or describe what kind of info the variable is holding
    - Names follow the camelCase rules, meaning if there are more than one word in your variable name, the first word is not capitalized but every subsequent word is capitalized with no spaces separating the words.  

  - A few examples of JavaScript reserved words that should be avoided in variable names include: function, while, return, native, continue, float, with, void, true, false, etc.  


4. How can an array be useful when dealing with multiple related values? How do you access/change a value in an array?

  - Array's are useful when dealing with multiple related values because it organizes them into a list that could be added to, subtracted from, and a host of other procedures.  They are helpful when not knowing how many items it will contain because you do not need to specify how many values it will hold.   
    Values in an array are accessed as if they are in a numbered list.  Each value is assigned an index value based on its position in the array.  These index values are zero-based meaning the first value in an array is 0, the second value is 1, and so forth.  You can access any value an array by its index value.  
        ```JavaScript
          var animals = [dog, cat, bird, snake];
          animals[2] = bird;
        ```


5. What is the difference between an expression and a statement?

  - A statement is an individual instruction or step that a computer can follow. An expression evaluates (results in) a single value.  Expressions have an assignment operator that results in a single value. Expressions can assign a value to a variable or can use two or more values to return a single value.
  ```JavaScript
      statement ex: var color;
      expression ex: var color = 'green';
      expression ex: var myFavColor = "My favorite color is " + color;
              // myFavColor variable would have a value of "My favorite color is green";
  ```

6. What are three types of operators and how are they used?

  - Assignment operators -> assigns a value using an equal sign
  - Arithmetic operators -> perform basic math functions (+, -, *, /)
  - String operators -> combine or concatenate two or more strings together using a '+'
  - Comparison operators -> compare two values and return a boolean response, true or false.  Examples are <, >, <=, >=, ===, ==, etc.
  - Logical operators -> combine expressions and return a boolean response, true or false.  Examples are && (and) and || (or) 
