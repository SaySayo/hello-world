CSS FLEXBOX

Css flexbox is used to align items to make them look better, it is written as display: flex; setting the display to flex automatically puts the flex items in a row view(displays items horizontally from left to right). A feature of flex is the flex direction and there are 4 kinds of directions, row default), column(displays items vertically from top to bottom), row-reverse(right to left) and column-reverse(bottom to top).
Sometimes your items do not fill out the flex container, so there are options to decide how you want to space your items. the justify-content property aligned flex items along the main axis. For rows, the main axis is a horizontal line and for columns it is a vertical line. The property justify-content gives several options to space them, namely center which is the default justify-content option, flex-start (aligns items to the start of the flex container), flex-end (aligns items to the end of the flex container), space-between(aligns items to the center of the main axis, with extra space placed between the items), space-around (the first and last items are not locked to the edges of the container, the space is distributed around all the items with a half space on either end of the flex container.) and space-evenly( Distributes space evenly between the flex items with a full space at either end of the flex container).

Flex containers also have a cross axis which is the opposite of the main axis. For rows, the cross axis is vertical and for columns, the cross axis is horizontal. CSS offers the align-items property to align flex items along the cross axis. For a row, it tells CSS how to push the items in the entire row up or down within the container. And for a column, how to push all the items left or right within the container. Options of the align-items are;
flex-start: aligns items to the start of the flex container. For rows, this aligns items to the top of the container. For columns, this aligns items to the left of the container.
flex-end: aligns items to the end of the flex container. For rows, this aligns items to the bottom of the container. For columns, this aligns items to the right of the container.
center: align items to the center. For rows, this vertically aligns items (equal space above and below the items). For columns, this horizontally aligns them (equal space to the left and right of the items).
stretch: stretch the items to fill the flex container. For example, rows items are stretched to fill the flex container top-to-bottom. This is the default value if no align-items value is specified.
baseline: align items to their baselines. Baseline is a text concept, think of it as the line that the letters sit on.

Flex-shrink and Flex-grow are used to control the sizes of items in their container by shrinking and growing.
The flex-basis property specifies the initial size of the item before CSS makes adjustments with flex-shrink or flex-grow. The units used by the flex-basis property are the same as other size properties (px, em, %, etc.). The value auto sizes items based on the content.
There is a shortcut available to set several flex properties at once. The flex-grow, flex-shrink, and flex-basis properties can all be set together by using the flex property. For example, flex: 1 0 10px; will set the item to flex-grow: 1;, flex-shrink: 0;, and flex-basis: 10px;
The order property is used to tell CSS the order of how flex items appear in the flex container. By default, items will appear in the same order they come in the source HTML. The property takes numbers as values, and negative numbers can be used.
The align-self  property allows you to adjust each item's alignment individually, instead of setting them all at once. align-self accepts the same values as align-items and will override any value set by the align-items property.
Flex-wrap is used to space out flex items into multiple lines. It accepts the following values:

nowrap: Every item is fit to a single line.
wrap: Items wrap around to additional lines.
wrap-reverse: Items wrap around to additional lines in reverse.

You can use align-content to set how multiple lines are spaced apart from each other. This property takes the following values:

flex-start: Lines are packed at the top of the container.
flex-end: Lines are packed at the bottom of the container.
center: Lines are packed at the vertical center of the container.
space-between: Lines display with equal spacing between them.
space-around: Lines display with equal spacing around them.
stretch: Lines are stretched to fit the container.
This can be confusing, but align-content determines the spacing between lines, while align-items determines how the items as a whole are aligned within the container. When there is only one line, align-content has no effect.
Flex-flow is a shortcut property for flex-direction and flex-wrap. E.g flex-flow: row wrap;

