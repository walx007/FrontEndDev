##### For more on Grid Layouts, see the below articles.  
- Creating complex Grid layouts [https://rachelandrew.co.uk/archives/2015/02/04/css-grid-layout-creating-complex-grids/]
- Nesting & overlapping of Grid items [https://gridbyexample.com/examples/example21/]


---------------------------------------------------------------------------------------------------

#### Media Queries
While media queries can be used for a variety of things and in a number of ways, we are going to focus on what are called **breakpoints**, which are the viewport width at which we want our design to change. We then write the code inside that media query, with a set breakpoint, that we want to go into effect only when the viewport width that the app is being viewed on is at least the breakpoint width. Only the CSS that we want to change needs to go here - the original CSS rules will all still apply, and only the new CSS rules written inside the media query will override any pre-existing rules.


**Key Term**
- **viewport** - the area of the window in which web content can be seen. We use the dimensions of the viewport (usually the width, but sometimes the height) as the basis of our media queries.

- For more information about viewport see  
- What is a viewport?  [https://developer.mozilla.org/en-US/docs/Web/CSS/Viewport_concepts#What_is_a_viewport]
- Using the viewport meta tag to control layout on mobile browsers [https://developer.mozilla.org/en-US/docs/Mozilla/Mobile/Viewport_meta_tag]


#### Multiple Breakpoints
We have seen how to set a breakpoint and use Media Queries to create different layouts for smaller screens and larger screens, but there are some development moments that will call for 3 possible layouts.


A simple example would be creating 2 different breakpoints so that up to x width one set of CSS rules apply, then between x and y width a second set would apply, and then for anything beyond a width of y a third set of CSS rules would apply.


Here is an example of what that code could look like:

' /* Anything smaller than first breakpoint 600px */
.container {
  // rules for small screen
}

/* Medium Screens */
@media (min-width: 600px) and (max-width:900px) {
  .container {
    // rules for medium-sized screen
  }
}

/* Large Screens */
@media (min-width:901px) {
  .container {
    // rules for large screen
  }
} '

