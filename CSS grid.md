CSS GRID
You can Turn any HTML element into a grid container by setting its display property to grid. I.e display: grid; To add some columns to the grid, use the grid-template-columns and set the value using px or em, i.e grid-template-column: 10px 10px; 
To add some rows to the grid, use the grid-template-rows and set the value using px or em, i.e grid-template-rows: 10px 10px; 
You can also set the value using the following units;
 fr: sets the column or row to a fraction of the available space,
auto: sets the column or row to the width or height of its content automatically,
%: adjusts the column or row to the percent width of its container.

To reduce repetition when defining the structure of a grid using grid-template-rows and grid-template-columns, you can use the repeat function. Here's an example that would create the 100 row grid, each row at 50px tall.
grid-template-rows: repeat(100, 50px);

Minmax is used to limit the size of items when the grid container changes size. To do this you need to specify the acceptable size range for your item. Here is an example:

grid-template-columns: 100px minmax(50px, 200px);
The repeat function comes with an option called auto-fill. This allows you to automatically insert as many rows or columns of your desired size as possible depending on the size of the container. You can create flexible layouts when combining auto-fill with minmax, like this:
repeat(auto-fill, minmax(60px, 1fr));
Auto-fit works almost identically to auto-fill. The only difference is that when the container's size exceeds the size of all the items combined, auto-fill keeps inserting empty rows or columns and pushes your items to the side, while auto-fit collapses those empty rows or columns and stretches your items to fit the size of the container.

Note: If your container can't fit all your items on one row, it will move them down to a new one


To add a gap between the columns, use the grid-column-gap property like this: grid-column-gap: 10px;
To add a gap between the rows, use the grid-row-gap property like this: grid-row-gap: 10px;
Grid-gap is a shorthand property. If it has one value, it will create a gap between all rows and columns. However, if there are two values, it will use the first one to set the gap between the rows and the second value for the columns. 
NB: the above grid spacing properties are for grid containers
Grid-column property is used to control the amount of column an item will consume in conjunction with the line numbers you want the item to start and stop at. E.g grid-column: 1/3; 
Grid-row property is used to control the amount of row an item will consume in conjunction with the line numbers you want the item to start and stop at. E.g grid-row: 1/3; 
Justify-self property is used to horizontally align individual grid items in its cell. The default option is stretch which fills up the grid with the item, other options are center, start and end.
A cell is the box where the content of each item is located in.
Align-self property is used to vertically align individual grid items in its cell. It uses the same options as justify-self
Justify-items property is used to horizontally align all the grid items in their cell. It uses the same options as justify-self.
Align-items property is used to vertically align all the grid items in the cell. It uses same options as align-self
Grid-template-areas property is used to group cells of grids together into an area. You can give the area a custom name. E.g 
grid-template-areas:
  "header header header"
  "advert content content"
  "footer footer footer";

You can place an item in your custom area by referencing the name you gave it. To do this, you use the grid-area property on an item like this:

.item1 {
  grid-area: header; 
}
