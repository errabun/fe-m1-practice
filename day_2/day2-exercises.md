**Chapters 3 & 4 questions**

1. There are three main types of lists in HTML: ordered, unordered, and definition. What are their differences?

  - An ordered list is a numbered list that typically contains a set of specific instructions to be following
  that order.  For example a cooking recipe.  Declare an ordered list by using `<ol>` element followed by your
  list items, `<li>`.
  - An unordered list prints a list of bullet points and is declared using the `<ul>` element followed by list
  items, `<li>` for each bullet point.  
  - A definition list typically uses pairs of definition terms, `<dt>` and their term definitions, <dd>.  The
  definition term (`<dt>`) element typically states the term that is going to be defined (`<dd>`).
  For example:
  ```Javascript
  <dl>
    <dt>Lit</dt>
      <dd> To be on fire or to be having loads of fun. </dd>
  </dl>
  ```

2. What is the basic structure of an element used to link to another website?

  - `<a href="http://www.facebook.com">Facebook Login</a>`

  Need to begin by using the `<a` element to tell browser you want to create a link, followed by the attribute
  href.  The value assigned to the element href is going to be the absolute url of the page you are linking,
  followed by the closing bracket for the link declaration.  The text that follows, in this case Facebook Login,
  is what is displayed as the link to be clicked on, followed by the closing element, `</a>`.

3. What attribute should you include in a link to open a new tab when the link is clicked?

  - When you want to open a new tab, you need to use the same format as the question above, but after you assign
  the href value (the absolute url of the page you wish to send user), you must add an additional attribute named
  target and set the value of the target attribute to "_blank". It is good practice to inform user that they will
  be redirected to a new window/tab.  

  Example: `<a href="http://www.google.com" target="_blank">Google</a> ` (opens in new window)

4. How do you link to a specific part of the same page?

  - In order to link to a specific part of the page you are on, you will need to access the id attribute
  associated with that part of the page.  The value of the id attribute can be called upon in as the value
  for the href attribute in your list element.  You must use a # tag before calling upon the id attribute value.

  Example:
  ``` Javascript
  <h1 id="top">Golf is Great!</h1>
  <a href="#fun_golf_courses">Where to play</a><br />  // example of how to link to a specific part of page
  <a href="#conclusion">Conclusion</a><br />
    <p> Golf is great for a variety of reasons. </p>
  <h2 id="fun_golf_courses"> Here is a list of golf courses</h2>
    <ul>
      <li>Scotland</li>
      <li>Mexico</li>
    </ul>
  <h3 id="conclusion"> So go play golf!</h3>
  <p><a href="#top">Back to top</a></p>
  ```

  **Chapters 10, 11, 12 questions**

1. What is the purpose of CSS?

  - The purpose of CSS is to be able to style the page.  It allows the developer to present web pages with different colors, layouts, fonts, etc.  It can also adapt a page for different browsers and types of devices that a user may be using.

2. What does CSS stand for? What does cascading mean in this case?

  - CSS stands for Cascading Style Sheets.  Cascading means that the developer can write simpler rules for styling because you can create generic rules that apply to most elements in an HTML document and override properties on individual elements that need to appear differently.  If 2 or more rules apply to the same element, the latter will take precedence.  As well, if one selector is more specific, the CSS rule associated with that selector will take precedence.  Lastly, you can also add `!important` to the property value to tell browsers it is more important than other rules with the same element.  


3. What is the basic structure of a CSS rule?

  - The basic structure of a CSS rule contains a selector and a declaration.  The selector defines what HTML element to be styled.  The declaration has two parts, a property and a value separated by a colon & indicate how selector(s) are going to be styled.  We are able to declare multiple selectors to follow the same declaration styling rules separated by a comma.  As well, we are able to have multiple values in our declaration separated by semi-colons.  

4. How do you link a CSS stylesheet to your HTML document?

  - When using an external CSS stylesheet in a HTML document, you must tell the HTML doc where to find the CSS file.  This should be designated in the `<head>` section in the HTML document. It must contain 3 attributes:
    1. href: specifies the path to the CSS file.
    2. type: specifies the type of document; should be 'text/css'.
    3. rel: specifies the relationship between HTML page and file it is linked to.  This value should be 'stylesheet' when linking a CSS file.

5. When is it useful to use external stylesheets as opposed to using internal CSS?

  - It is best use to use an external stylesheet when you have more than 1 page on a site.  This allows all pages to follow the same style rules without having to repeat code for every page.  As well, it keeps content separate from how the page works.  Developers can change styles used across all pages by altering just one file instead of changing styling for each page of a site.  
  When using internal CSS, you are able to place CSS rules directly in the HTML document inside `<style>` elements that are located in the `<head>` of the HTML document. Mostly used for smaller, 1 page HTML documents, and for rules that will apply to the entire page.  

6. Describe what a color hex code is.

  - Color hex code is 6 digit code that represents the amount of red, green and blue in hexadecimal code.  It is preceded by a # sign and contains letters and numbers. The first two values indicate the amount of red, the second two values indicate amount of green and the last two values indicate the amount of blue to be displayed.  For example:
  `#66cdaa`

    66 represents a red value of 102; cd represents a green value of 205; and aa represents a blue value of 107.

7. What are the three parts of an HSL color property?

  - The three parts of an HSL color property are hue, saturation and lightness.  Hue is often represented as a color wheel with values from 0 to 360.  Saturation is the amount of grey in a color and is represented as a percentage with 100% being full saturation and 0% is a shade of grey.  Lightness is the amount of black or white in a color and is also represented as a percentage with 100% being white and 0% is black.

8. In the world of typeface, what are the three main categories of fonts? What are the differences between them?

  - The three main categories of fonts in CSS are serif, sans-serif and monospace.  Serif fonts have small, extra details on each of the letters.  Sans-serif have all straight ends to letters, typically a little cleaner design.  Lastly, monospace displays letters with the same width.  

9. When specifiying font-size, what are the main three units used?

- The three main units used when specifiying font-size in CSS are pixels, percentages and ems.  Pixels are the most commonly used and are the number of pixels followed by px.  Percentages depend on the default size of the text in the browser. Most browsers are 16px,  so 75% would be equvalent of 12px.  An em is equivalent to the width of the letter m. One example could be written as `font-size: 1.3em;`. 
