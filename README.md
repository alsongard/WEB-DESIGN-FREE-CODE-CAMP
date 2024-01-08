# FREECODE CAMP WEB DESIGN
************************************************************************
## FREECODE CAMP LESSONS
>> ### COLOR PROPERTIES

************************************************************************
### COLOR
#### color properties:
* hsl() - takes in 3 arguments one for hue,saturation and lightness. lightness and saturation are given in percentage.

* hex value uses 6 values 1 pair representing each main color code RGB it starts with #00FF00 FF means 100% of color, 00 is 0% of color.

* rgb() is also used for setting the color property, it takes in 3 arguments each representing the 3 main color codes having values between 0-255.

* linear-gradient - works with background{} property. It takes in 3 arguments the first being the degree of change and the secong and third being the color to change from and to second color.
E.g changes from red to green with a 90 deg change 
``background:linear-gradient(90deg, rgb(255,0,0),rgb(0,255,0)) `` 
it can also take another argument, also color stops.

example:
class name = "mine"
.mine background:linear-gradient(180, hsl(75,55%,89%)50%/*stop*/, hsl(10,88%,22%),hsl(80,52%,89%))
by default the line is 180 degree change.
DIV
div elements have a block property: take the space of the whole line
BORDER
the border propery is used for designing the border of an element and one can decide which side to be applied.
border-left, border-right , border
border-left(size type color) it takes in 3 arguments size given in px(pixel value) , type can be solid , double and color for color.
#BOX-SHADOW
add a shadow for an element
it can take up 4 arguments
box-shadow : offsetX offsetY blurRadius Color;
box-shadow : 5px 5px 5px Green;
it can take up 5 args
box-shadow:offsetX offsetY blurRadius spreadRadius Color;

# CSS FLEXBOX
***********************************
## border-box propery
the border-box propery uses 2 models one  being content-box and the other border-box.With content-box which is the default is, padding and margin values are added to the with of the element content e.g img while with the border-box model the entire width is calculated by adding both the padding,margin and width of the content.

## flexbox
The flexbox has 2 axis mainly the main axis and the cross axis.
the main axis which is the flex-direction property can take in 4 values that define the direction of the flex items or of the flex container.
>> these are :
>>> * column 
>>> * column-reverse
>>> * row(default)
>>> * row-reverse
 
## wrap
the wrap method is used to push elements to the next line ``flex-wrap:wrap;``. However this can be removed by assiging ***none***.

## submit
When using the submit button ensure to set the height to place the value | text submit to center