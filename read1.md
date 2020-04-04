# Responsive Web Design:
## Responsive Overview:
 the practice of building a website suitable to work on every device and every screen size.
 ### Responsive vs. Adaptive vs. Mobile:
  Responsive: means to react quickly and positively to any change, *websites continually and fluidly change based on different factors, such as viewport width*
  adaptive: means to be easily modified for a new purpose or situation, such as change.
*websites are built to a group of preset factors*
#### A combination of the two is ideal, providing the perfect formula for functional websites.
# Flexible Layouts:
 ##### flexible layouts:
  is the practice of building the layout of a website with a flexible grid, capable of dynamically resizing to any width.
  ##### Flexible grids:
   are built using relative length units, most commonly percentages or em units.

   ### Media Queries: 
   Media queries were built as an extension to media types commonly found when targeting and including styles.
# What is “Float”?
Float is a CSS positioning property. To understand its purpose and origin.
In web design, page elements with the CSS float property applied to them are just like the images in the print layout where the text flows around them.
## What are floats used for?
floats can be used to create entire web layouts, Floats are also helpful for layout in smaller instances.

### Clearing the Float:
Float’s sister property is clear. An element that has the clear property set on it will not move up adjacent to the float like the float desires.

*Clear has four valid values as well. Both is most commonly used, which clears floats coming from either direction. Left and Right can be used to only clear the float from one direction respectively. None is the default, which is typically unnecessary unless removing a clear value from a cascade.*

#### Problems with Floats:
1. Pushdown is a symptom of an element inside a floated item being wider than the float itself (typically an image).
2. Double Margin Bug.
3. 3px Jog 
4. Bottom Margin Bug

### Context:
A block level element is as wide as the parent it’s inside (width: auto;)
### Clearing Context:
The parent element will collapse to zero height since it has only floated children.
.grid:after {
  content: "";
  display: table;
  clear: both;
}
# Gutters:
grid are flexible by using percentages for widths, 
