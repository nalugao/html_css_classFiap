# html_css_classFiap
This project was developed during a college class to practice the fundamentals of HTML and CSS, focusing on responsive design and layout structuring. 
<a href="https://youtu.be/p3q5v4rjNsk">Check out the Landing Page on YouTube.</a>

<h2>Lessons learned:</h2>
<h4>Class</h4> In CSS, a class is a way to apply styles to one or more HTML elements. Classes allow you to group elements and style them consistently without affecting other elements.
<li>A class is defined in CSS with a dot (.) followed by the class name.
<li>In HTML, you apply a class to an element using the class attribute.</li>
<li>Multiple elements can share the same class.</li>
<li>An element can have multiple classes.</li>

<h4>:root</h4> is a pseudo-class selector that represents the root element of the document, which in the case of an HTML page is always <html>. <br /> It is commonly used to define CSS variables (also called custom properties), because anything defined in :root is available throughout the entire document, acting like a "global scope."

For exemple:

<ul type="square">
  <li>Variables --main-color, --secondary-color, and --default-font are defined globally in :root.</li>

  <li>Anywhere in your CSS, you can use them with var(--variable-name).</li>

  <li>Updating a variable in :root automatically updates all places where it’s used.</li>
</ul>
<code>
:root {
  --main-color: #3498db;
  --secondary-color: #2ecc71;
  --default-font: 'Arial', sans-serif;
}

body {
  background-color: var(--main-color);
  font-family: var(--default-font);
  color: white;
}

h1 {
  color: var(--secondary-color);
}
</code>

<h4>Reset CSS</h4> It's important to reset all the default browser styles so they don't affect your code. The * selector targets all elements in the HTML.

For example:

<code>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box; /*por padrão, colocar sempre no reset*/
    font-family: "Quicksand", sans-serif;
  }
</code>

<h4>text-wrap: balance;</h4> automatically balances text lines to avoid awkward word breaks on different screen sizes
<h4>background-size: cover;</h4> stretches the image to fill the entire screen
<h4>background-position: 50%;</h4> or "center", always keeps the center point of the image visible according to responsiveness
