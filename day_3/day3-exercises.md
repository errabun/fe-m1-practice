***Chapter 7 - Forms***

1. If you're using an input element in a form, what attribute controls the behavior of that input?

  - The type attribute controls the behavior of that input.  There are several different values of form control,
  they can be declared using the type attribute assigning the value to which form control is best suited for
  the situation.


2. What element is used to create a dropdown list?

  - The dropdown list box or select box allows users to select one option from a dropdown list.  
  We use the `<select>` option to declare the dropdown list.  Inside the `<select>` option we delcare
  the different options using the `<option>` elements with value attributes that log the selection to
  the server.  See example below:
  ```
  <form action="http://www.example.com/profile.php">
    <p>
      <label for="preferred-tv">
        What is your preferred way to watch television:
      </label><br />
    <select name="devices" id="preferred-tv">
      <option value="cable"> Cable </option>
      <option value="internet"> Internet Streaming </option>
      <option value="none"> I don't like TV </option>
    </select>
    </p>
    ```

3. If you're using an input element to send form data to a server, what should the type attribute be set to?

  - When sending form data to a server, the type attribute should be set to "submit".  This form control will create a text
  box and a 'submit' button.  Depending on the type of information that is being collected, you are able to include
  a name attribute (not necessary) and a value attribute.  The value attribute will show the text you wish to display on the
  submit button.  It is good practice to include the value attribute to show the appropriate response to the kind of form.
  

4. What element is used to group similar form items together?

  - The `<fieldset>` element is used to group similar form items together.  The `<fieldset>` element places a line/box around
  the edge to show that each form element is related. Inside the `<fieldset>` element, it is good practice to include a
  `<legend>` element which shows a caption identifying the purpose of that group of form controls.  



***Chapters 13 & 15 - Boxes and Layout***

1. Describe the differences between border, margin, and padding.

  - The every element in an HTML document has a border, even if not visible (0px).  Each element is thought of to be in a box, and the outside of that box is the border of that element.  The space between the content in the HTML document and the border is called the padding.  It is the space between the border of box and the content within it.  Lastly, the margin is the space outside of the box.  The live outside the edge of the border.  


2. For a CSS rule padding: 1px 2px 5px 10px, what sides of the content box does each pixel value correspond to?

  - For CSS rule padding the numbers that are listed go in clockwise order beginning at the top.  So the order of the padding would be 1px from the top, 2px from the right side, 5px from the bottom, and 10px from on the left side.


3. Describe the difference between block-level and inline elements.

  - Block-level elements are displayed on top of one another.  So the first element would be at the top, second a space below that, and so forth.  Block elements are more like a condescending list from top down. Inline elements are displayed side by side from one another and mostly require setting a margin-right property to allow space from one another.  They are displayed as if you are reading them from left to right.  


4. What is the role of fixed positioning, and why is z-index important in the scenario of using fixed positioning?

  - Fixed positioning is a type of absolute positioning where the element is fixed on the page and does not move when the user scrolls up or down the page in the browser window.  Seeing as the element doesn't move when user scrolls, some elements are bound to overlap.  The z-index allows the developer to control which element sits on top of the overlapping elements.  It is a number and the higher the number, the closer that element is to the top.  Improves readability.  

5. What is the difference between a fixed and liquid layout?

  - The elements on a fixed layout do not change in size when user increases or decreases the size of a window.  Seeing as the elements are fixed, they are typically listed in pixels. Whereas liquid layouts stretch and contract as the user increases or decreases the size of the browser window. Liquid layouts typically are listed as a percentage.  Both have pros and cons depending on the type of page and the amount of content on the page.  
