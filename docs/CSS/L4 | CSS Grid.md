#### CSS Grid vs Flex 
> grid layout enables an to align elements into columns and rows and it's 2-d. 
Flexbox is for how content flows, Grid is for how content is placed -
i.e. grid works nicely for page layouts, flex works nicely for regions within the grid.  

> To use CSS Grid set the display property of the container element to grid.

- CSS Grid v. Flexbox  
 - Grid is two dimensional, while Flex is one  
 - Grid is layout first, while Flexbox is content first  
 - Flex is for components of an app, Grid is for the app layout itself.  
 
CSS Grid does not replace Flexbox.They work really when each other.  
- At the highest level CSS Grid excels at creating layouts for a webpage, while Flexbox is a master of content flow for each element that makes up the page layout.  

- https://medium.com/youstart-labs/beginners-guide-to-choose-between-css-grid-and-flexbox-783005dd2412  
- https://hackernoon.com/the-ultimate-css-battle-grid-vs-flexbox-d40da0449faf  
- https://css-tricks.com/css-grid-replace-flexbox/


--------------------------------------------------------------------------
#### Rows & Columns | `grid-template-columns` and `grid-template-rows`
A CSS Grid is made up of rows and columns which are defined using the CSS properties `grid-template-columns` and `grid-template-rows`, which take as values the size of each track.

-----------------------------------------------------------------
#### grid-area
The grid-area property specifies a particular area or set of rows and columns that a grid item occupies. It is applied to the grid item itself with CSS. Here is an example:

```.item{grid-area: 1/2/3/3}```  
> Because grid-area is shorthand for the properties: grid-row-start, grid-column-start, grid-row-end and grid-column-end, the code above places the item from rows 1-3, and columns 2-3.  

- Working with Grid Areas  
  - The grid-area property defines the space an element takes up in the grid by setting values for the row it starts and ends in, and the column it starts and ends in. In practice it could look like this:  
  ```#one {  /* row start/column start/ row end/ column end */grid-area: 1/2/3/3;}```  
  In this example the element with the id, one would start at the first row and the first column, and end at the third row (which is the end of the second row if there is no third row) and the third column.
  
  --------------------------------------------------------------------------------------
  #### grid-template-areas 
 -  Grid Areas Summary  
 grid-template-areas is the property used to name the rows and columns of a grid and to set its layout. It could look like this:  
 
 ```.container {display:grid;grid-template-columns: 300px 300px 300px;grid-template-rows: 250px 600px; grid-template-areas: "hd hd hd hd hd hd hd hd""sd sd sd main main main main main""ft ft ft ft ft ft ft ft";```
  }  
  Thenamed areas in the grid are then assigned to each element according to where you want them to be displayed in the grid:

```.header {grid-area: hd;}```  
In the example above the element with the class header will stretch across the entire first row of columns because we have assigned it the grid-area hd, and we have defined the area hd with the value for grid-template-areas in the parent element

------------------------------------------------------------------------------------------------------------------------------------
#### Advanced Grid
CSS Grid includes advanced capabilities for creating large and complex grids. Some of these are:  
- the fr Unit  -it is used to fill rest of space.
- Track listings with `repeat()` notation  
- Track sizing and `minmax()`-use it in combination with `grid-auto-rows` to generate the infinite rows.e. fb feed.

