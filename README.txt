1. The box-sizing property is used to set the way browsers calculate the size of containet element. By default, content-box model is used, when an element has a specific width, that width is calculated based only on the element's content. Padding and border values get added to the total width, so the element grows to accommodate these values.
Try setting box-sizing to content-box explicitly, with the global * selector. At this point, you will not see any changes, because you are using the default value.

2. The border-box sizing model does the opposite of content-box. The total width of the element, including padding and border, will be the explicit width set. The content of the element will shrink to make room for the padding and border.
Change the box-sizing property to border-box.

3. Make the text uppercase using the text-transform property with uppercase as the value.

4. Flexbox is a one-dimensional CSS layout that can control the way items are spaced out and aligned within a container.
To use it, give an element a display property of flex. This will make the element a flex container. Any direct children of a flex container are called flex items.

5. Flexbox has a main and cross axis. The main axis is defined by the flex-direction property, which has four possible values:
    row (default): horizontal axis with flex items from left to right
    row-reverse: horizontal axis with flex items from right to left
    column: vertical axis with flex items from top to bottom
    column-reverse: vertical axis with flex items from bottom to top
Note: The axes and directions will be different depending on the text direction. The values shown are for a left-to-right text direction.

6. Flex-wrap property determind how your flex behave when the flex container is too small. Setting it is wrap allow the items to wrap to the next row or column. Nowrap is prevent item wrap to the next row or column.

7. justify-content determind how your items inside flex-container is positioned along the main axis. affecting their position and the space around them.

8. otice how some of your images have become distorted. This is because the images have different aspect ratios. Rather than setting each aspect ratio individually, you can use the object-fit property to determine how images should behave.
Give your .gallery img selector the object-fit property and set it to cover. This will tell the image to fill the img container while maintaining aspect ratio, resulting in cropping to fit.

9. The gap CSS shorthand property sets the gaps, also known as gutters, between rows and columns. The gap property and its row-gap and column-gap sub-properties provide this functionality for flex, grid, and multi-column layout. You apply the property to the container element.

10. The ::after pseudo-element creates an element that is the last child of the selected element. You can use it to add an empty element after the last image. If you give it the same width as the images it will push the last image to the left when the gallery is in a two-column layout. Right now, it is in the center because you set justify-content: center on the flex container.
