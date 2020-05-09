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

#### Specificity in CSS

Because elements can have multiple CSS selectors, there is a hierarchy for the weight given to each type of selector. Here is the logical order of selectors from least to most weight assigned:  

- Type selectors (e.g., h1) and pseudo-elements (e.g., ::before).  
- Class selectors (e.g., .example), attributes selectors (e.g., [type="radio"]) and pseudo-classes (e.g., :hover).  
- ID selectors (e.g., #example). 
This concept can help you understand why your styles aren't being applied in the way you expect.  

-There is a way to escape or override the specificity evaluation of elements using the !important keyword after an individual CSS property rule, but a couple important reminders:

Always look for a way to use specificity before even considering !important. Never use !important on site-wide CSS.

-------------------------------------------------------------------------------

#### The Box Modal  
- The box model is the basic building block of CSS.  
- According to the box model concept, every element on a page is a rectangular box and may have width, height, padding, borders, and margins.  
- When a browser renders (draws) a webpage each element, for example a piece of text or an image, is drawn as a rectangular box following the rules of the CSS Box Model.  

##### Padding  
* Next is padding - the space between the box’s content and its border. Note that padding is in addition to the content’s height and width, and is considered to be inside the element itself.

##### Margin  
* Last is the margin, which surrounds the rest of the box. It is the space between the box and surrounding boxes.  

-----------------------------------------------------------------------------------

#### Display and Positioning: Inline & Block  
* Each element can have an inside display and outside display property.  
- Inside Display- It determines the positioning behaviour of children inside parent element.{Ex.Flexand Grid}.  
We will dicuss about Inside Display later and now we will see how outer display works.  
- `display:block`-In the CSS code if we set the box class display property to block, each rectangle would take up its own line and would be positioned one on top of the other.  
- `display:inline-block`-if we set the display property to inline-block, the rectangles would be displayed side by side on the same line. Here is what the CSS could look like.
- `display:inline`- The value inline is most often used to highlight specific text within a larger text element, span elements are a common example. Elements set to inline display have no width or height and only occupy the space that their text property (or .innerHTML property) takes up.
