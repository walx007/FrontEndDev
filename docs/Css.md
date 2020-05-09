### 1) CSS Psuedo Classes.
A CSS pseudo-class is a keyword added to a selector that specifies a special state of the selected element(s). For example, :hover can be used to change a button's color when the user's pointer hovers over it.

/* Any button over which the user's pointer is hovering */
button:hover {
  color: blue;
}
Pseudo-classes let you apply a style to an element not only in relation to the content of the document tree, but also in relation to external factors like the history of the navigator (:visited, for example), the status of its content (like :checked on certain form elements), or the position of the mouse (like :hover, which lets you know if the mouse is over an element or not).

Note: In contrast to pseudo-classes, pseudo-elements can be used to style a specific part of an element.

Syntax
selector:pseudo-class {
  property: value;
}
Like regular classes, you can chain together as many pseudo-classes as you want in a selector.

------------------------------------------------------------------------------------------------------
#### Linking two css files
So you’ve just learned that using the <link> element allows you to link HTML and CSS files together. What about linking a CSS file to another CSS file? You can have all your styles living inside one main CSS file, or you can use @import to break your styles (one for layout, one for images, one for blog cards, etc.) into a number of smaller, focused files. This makes it a lot easier to manage the styles they contain and your code is more scalable and modular!

// at the top of your main CSS file

@import “./layout”;
@import “./images”;
@import “./blog-cards”;
-----------------------------------------------------------------------------------
