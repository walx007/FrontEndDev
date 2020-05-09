https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout/Flexbox  

### the Flexible Box Module CSS  
Flexbox is a one-dimensional layout method for laying out items in rows or columns. 
Items flex to fill additional space and shrink to fit into smaller spaces.  

Flexbox (the Flexible Box Module) is a set of CSS rules for stretching multiple columns or rows across a parent container. 
 Flex is unique amongst CSS properties because you have a main container and the items nested within it. CSS flex has properties that 
 apply to both the element itself, and the items inside of it.  
 
 * To use flexbox set the display property of the parent container to flex:

``` .container{ display:flex; }```


>Before the Flexbox Layout module, there were four layout modes:  
> - Block, for sections in a webpage  
> - Inline, for text  
> - Table, for two-dimensional table data  
> - Positioned, for explicit position of an element.  
The Flexible Box Layout Module, makes it easier to design flexible responsive layout structure without using float or positioning.




#### FlexBox  - The css Flex box module specilizes in *aligning* and *distributing* elements within a parent element.

The alignment and justification can be made easliy by softwares (illustrator), but untill flex box it was difficult to align and distrubite elements 
in a appealing way just by code.  
- The flex container can expand to fit items/children elements inside it.  
- To use flexbox set the display property of a div to flex. The items inside that element will automatically become flex items, and you can then use the flexbox syntax in your CSS code.  
--------------------------------------------------------------------------------------
#### Axes and Direction with Flexbox   | `flex-direction: row`  

The Flexbox model relies on two axes: the main axis and the cross axis. The main axis is defined by flex-direction, which has four possible values:  
- row  
- row-reverse  
- column  
- column-reverse  
The two row settings will create the main axis horizontally - or inline direction. The two column settings will create the main axis vertically - or block direction. block or inline here refer to the CSS display settings which we have covered previously.

#### Ordering Elements with Flexbox | `order:value`  
There are three ways to explicitly set the order in which items will appear in a grid.  
1. Moving the HTML code for the elements themselves to reorder  
2. Appending -reverse to row or column will reverse the order in the specified row or column  
3. Using the order property of the individual items inside the grid
------------------------------------------------------------------------------------
#### Aligning Items & Justifying Content with Flexbox
align items--> It aligns items on the *cross* axis. use align-items with the possible values:
- stretch  
- flex-start  
- flex-end  
- center

``justify-content`` -To justify content on the *main* axis use justify-content, which has the possible values:

flex-start
flex-end
center
space-around
space-between
space-evenly

