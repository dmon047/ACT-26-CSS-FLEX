# ACT-26-CSS-FLEX
WHAT IS CSS FLEX BOX?
CSS Flexbox (short for Flexible Box Layout) is a layout model in CSS that allows you to design complex and 
responsive web layouts with ease. It provides a more efficient and flexible way to arrange elements within a container,
especially when dealing with elements of varying sizes or when the layout needs to adjust dynamically to different screen sizes.

.container {
  display: flex;
}

Flex Items: The child elements inside a flex container. They are automatically arranged along the main axis (horizontal by default), 
and can adjust their size and position based on the container's space.

Main Axis & Cross Axis:

The main axis is the axis along which flex items are placed. By default, it's horizontal (left to right), 
but it can be changed to vertical using the flex-direction property.
The cross axis is perpendicular to the main axis (vertical by default if the main axis is horizontal).

Flex Direction: This property defines the direction in which flex items are arranged along the main axis. The default is row (left to right). It can also be set to:

row: Items are arranged horizontally (default).
column: Items are arranged vertically.
row-reverse: Items are arranged horizontally but in reverse order.
column-reverse: Items are arranged vertically but in reverse order

Justify Content: Aligns items along the main axis. Common values are:

flex-start: Align items at the start of the container.
flex-end: Align items at the end of the container.
center: Center items.
space-between: Distribute items evenly with no space at the ends.
space-around: Distribute items evenly with space before and after each item.

Align Items: Aligns items along the cross axis (perpendicular to the main axis). Common values are:

flex-start: Align items to the top (if flex-direction is row).
flex-end: Align items to the bottom (if flex-direction is row).
center: Center items along the cross axis.
stretch: Stretch items to fill the container (default behavior).
baseline: Align items to their baseline.

Align Self: Overrides align-items for individual flex items.
It allows you to set different alignments for specific items in the container.

Flex Grow, Flex Shrink, and Flex Basis:

flex-grow: Defines how much an item can grow relative to other items if there's extra space in the container.
flex-shrink: Defines how much an item can shrink relative to other items if there is not enough space in the container.
flex-basis: Defines the initial size of an item before space distribution happens. It can be set to a specific length or auto.

Flex Wrap: By default, flex items are placed in a single row (or column). If you want items to wrap onto the next line when there is not enough space, use the flex-wrap property.

nowrap: Items will not wrap (default).
wrap: Items will wrap to the next line.
wrap-reverse: Items will wrap in the reverse direction.

.container {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-items: center;
}

.item {
  flex: 1 1 200px; /* Grow, shrink, basis */
  margin: 10px;
}

In this example:

The .container is a flex container with flex-wrap allowing items to wrap when necessary.
Items inside the container have a flexible width, meaning they grow and shrink based on the available space, with an initial size of 200px.

Why use Flexbox?
Responsive Design: Flexbox makes it easy to create responsive layouts that adjust to different screen sizes.
Alignment: It simplifies vertical and horizontal alignment of elements, which used to be difficult with traditional CSS.
Flexibility: It provides more control over how items behave, such as distributing space, growing, shrinking, or wrapping.
Flexbox is widely supported in modern browsers and is a powerful tool for building web layouts.

