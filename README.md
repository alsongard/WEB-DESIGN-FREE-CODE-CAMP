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
the border-box propery uses 2 models one  being content-box and the other border-box.With content-box which is the default is, padding and margin values are added to the width of the element content e.g img , while with the border-box model the entire width is calculated by adding both the padding,margin and width of the content.

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

## CSS POSITIONING
positioning propery allows a user to place elements / position an element in a webpage. It can take 4 properties namely:
static, fixed, absolute, relative and sticky
Once you set the position propery for the element you can move it by setting the top,right,bottom,left properties in pixels or percentage
the defualt position propery of elements is static and with these the element cannot be moved
observation: did not affect the position even with top and left propery set.
relative element:The element is still position to the normal flow of the document, but the top,left,right and bottom properties become active.
absolute property: with the absolute property the element is taken off the normal document flow and it's positionis dtrmnd by the top, right, left and bottom properties
fixed property: the fixed property makes an element to remian at it's position no matter the changes done to the width or the user scrolls
observation: the element does not move even in scrolling in takes the same top,left values 
sticky property: sticky property is a combination of both the fixed and realtive property. it remain to that position even if u scroll however it is not fixed
One way to center an item horizontally is to first:
set the position of the element to absolute:, set th etop,bottom,left,right to 0 and then set margin to auto;

## PSEUDO-SELECTORS
### not() pseudo-selector
pseudo-selector used to select elements that do not have the specified class. e.g
`` span:not(.sr-only) `
`will select all span elements that do not have the class .sr-only

### attribute target selector
the attribute target selector - it nonly selects elements that have a target attribute with a specific value. e.g
``span[class~="sr-only"] {...}``
the above code will only select span which have the class sr-only and not any other names

### !important
the !important keywork ensures that the styles of an element are not overwritten.E.g
``tr[class="total"]{
    color:#fff !important
}``

### nth-of-type()
the nth-of-type is a pseudo-selector that only selects an element based on its index value of the number. E.g
``span:nth-of-type(3){..}``
will select only the span element which is the third

### last-of-type
the last-of-type will select the last element of the element specified
``span:last-of-type{..}``
will select the last element of span
### first-of-type
It is used to select the first appearance of the element
``span:first-of-type{..}``
## Centering elements in a page
to center an element in a page, one can use the following options
### setting margin
for the margin, use
``margin:0 auto``
### setting position
set the position the absolute, and ensure the top,right,bottom,left values are 0.
>>```position:absolute;
>>top:0
>>right:0
>>bottom:0
>>left:0

### CSS VARIABLES
To declare a css variable use the syntax    ``--variableName-property:value``
```root:{
    --builing-color:rgb | hsl | color;
}
```
to use the variable name use the syntax ``var(--variableName)``
example:
```
    .home{
        background-color:var(--builidng-color);
    }
```