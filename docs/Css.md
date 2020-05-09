1) CSS Psuedo Classes.
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
