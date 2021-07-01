# CSS Template
This project was built to be all of my best practices I've picked up from my journey learning CSS.

## Style Guide
The #1 rule of maintainable code is that it should be readable and understandable.

> Code is more often read than it is written. ~ Robert C. Martin

### Element names come first
CSS is used on HTML elements to style them. CSS also can use component classes or utility classes.

This is important to point out because I believe the best solution is to give readable names to html elements to know what the element is that your working on is.

If an HTML element is to have a component class given to it (e.g., `nav-link`), that class should come first in the elements class list. 

For example: 

Good: Component class `nav-link` is at the beginning of the elements class list, so it's easy to tell what the element is that you're editing.
```
<a class="nav-link bg-dark text-green" href="home">Home Page</a>
```
Bad: Component class `nav-link` isn't first in the class list so you have to search to see what the elements represent.
```
<a class="text-green bg-dark nav-link" href="home">Home Page</a>
```
Of course, the general surrounding elements in your CSS should give you a hint of what the elements intention is.

Notice I said **if you are to include a component name** do the above. I didn't say "*you have to*."