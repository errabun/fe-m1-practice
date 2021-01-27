***Chapter 5 - Images HTML***

1. In an image element, why is the alt attribute important?

  - The alt attribute describes the image that is being displayed on the webpage.  It is important to include the alt attribute so it can be understood by screen reader software and search engines.  


2. What determines if an image element is inline or block?

  - Where the image is written in the HTML code determines if an image is inline or block.  If image is followed by another block element such as `<p>`, it will appear in block format in its own box with the following elements on a line below.  Inline elements sit within a block level element and do not start a new line.  When you place an image inside a block element such as `<p>`, the element will be wrapped into the text of that block element.  


3. What are the benefits of jpg or png image file formats?

  - It is best to use jpg file format for images with lots of different colors.  png files are best suited for images that have few different colors or images with a large area of the same color.


  ***Chapter 16 - Images CSS***


1. What is the benefit of specifying the height and width of images in CSS compared to specifying in the HTML?

  - It is beneficial to specify the width and height in CSS because you can control the width and height properties like any other element box.  This helps the page load more smoothly when loading the page because browsers will leave that load that space while waiting for the image to download. Whenever you use consistently sized images on page, it is best to use CSS to control the dimensions, instead of putting them in HTML. 


2. What is an image sprite, and why is it useful?

  - An image sprite is when a single image is used in different parts of the page, such as a logo.  It is useful because the browser only needs to download one image instead of several, making your page be able to load smoothly and efficiently.
