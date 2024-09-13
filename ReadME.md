<!--


=============================================================CSS TOPICS===============================================================
CSS Covered: -
  1.What is CSS?
  2.How to Apply CSS in html file?
  3.Syntax
  4.Selectors
  5.Specificity
     inline style - High Priority - 1000 Points
     id - 100 - priority Value
     class - 10 - priority value
     h1, p, div - 1

  6.Extensions
  7.Colors(RGB, RGBA, HSL, HEX)
  8.Background
  9.Borders
  10.CSS Typography
  11.Font Weight
  12.Font Style
  13.Text Transformation
  14.Text Decoration
  15.Leading
  16.Box Model
  17.PsedoElement
  18.Pseudo-classes
  19.Shadow(Text Shadow and Box Shadow)
  20.Float
  21.Positions
  22.Flex
  23.Grid
  24.Filter
  25.Linear Gradients - Not Covered
  26.Display
  27.Lists
  28.Tables - Not covered
  29.CSS Units - Not Covered
  30.Animations - Not Covered
  31.Transform(2D and 3D) - Not Covered
  32.Transition - Not Covered
  33.Box Sizing - Not Covered
  34.Media Queries - Not Covered
  35.CSS Variables - Not Covered

  =============================================================CSS Basic Styles============================================================
CSS Typography
  Font Families
   Serif
   Sans Serif
   Mono Space
   Cursice
   Display/Fantacy
  Font Weight, Style

Font Weight
 Normal
 Bold
 Bolder

Font Style
  Normal
  Italic
  Oblique


Text Transformation
 UpperCase
 LowerCase
 Capitalize


Text Decoration
  None
  Underline
  Overline
  LineThrough
  Blink


Leading
  Lineheight
  LetterSpacing
  WordSpacing



==============================================Box Moedl=========================================================================
Box Model:
  Margin - Clears an area outside the border. The margin is transparent
  Border - A border that goes around the padding and content
  Padding - Clears an area around the content. The padding is transparent
  Content - The content of the box, where text and images appear

===============================================Psedo Class and Psedo Elements====================================================


PsedoElement:(pseudo-element can only be applied to block-level elements)
  ::first-line
  ::first-letter
  ::before
  ::after
  ::marker
  ::selection


Pseudo-classes:
  Style an element when a user mouses over it
  Style visited and unvisited links differently
  Style an element when it gets focus

  Properties:
    :link - /* unvisited link */
    :visited - /* visited link */
    :hover - /* mouse over link */
    :active - /* selected link */


=========================================================Shadow=====================================================================
Text Shadow:
  text-shadow: 2px 2px 5px red;
  horizontal shaow, vertical shadow, blur and color


CSS Box Shadow:
  box-shadow: 10px 10px 5px lightblue;
  Same as Box shadow


==========================================================================LayOuts=====================================================

  Flex
  Grid
  Float
  Position

 1.Float:
    float: right;
    float: left;
    float: none;



 2.Positioning
    1.Static - Default Position
    2.Sticky - An element with position: sticky; is positioned based on the user's scroll position.
    3.Fixed - it always stays in the same place even if the page is scrolled
    4.Absolute - An element with position: absolute; is positioned relative to the nearest positioned ancestor (instead of positioned relative to the viewport, like fixed).
    5.Relatvie - An element with position: relative; is positioned relative to its normal position.
    6.Z-index - When elements are positioned, they can overlap other elements.

 3.Flex - One Dimensional Layout Design
    *need to first define a flex container.
       display: flex; - Container
     Flex Container:
      1.flex-direction - Values(column, column-reverse, row, row-reverse)
      2.flex-wrap - Values(wrap, no-wrap, )
      3.flex-flow - Shorthand propert of flex-direction and flex-wrap. Values(flex-direction, flex-wrap)
      4.justify-content - Align the flex-items. Values(center, flex-start, flex-end, space-around, space-between, space-evenly)
      5.align-items - Also Align the Flex Items. Values(center, flex-start, flex-end, stretch, baseline)
      6.aligncontent - Align the flexlines. Values(space-between, space-around, stretch, center, flex-start, flex-end)
     Flex Items: Child elements of flex container
      1.order - Order of the flex items. Values(order:1,...)
      2.flex-grow - How much flex items will grow relative to the rest of the flex items. Values(flex-grow: 1,....)
      3.flex-shrink - he flex-shrink property specifies how much a flex item will shrink relative to the rest of the flex items.
      4.flex-basis - The flex-basis property specifies the initial length of a flex item.
      5.flex - The flex property is a shorthand property for the flex-grow, flex-shrink, and flex-basis properties. Values(flex: 0 0 200px)
      6.align-self - Align the selected items inside the flex container it over rides the default alignment set by the align items to    the container Values(center, flex-start, flex-end)

 4.Grid - Two Dimensional Layout Design
   Grid Contaienr - display:grid;
   grid-template-column : measurements and how much column need;
   if three ratio, grid-template-column: 1fr 1fr 1fr; or auto
   Gap:
   column-gap:
   row-gap:
   gap

   Justify Content: Align the whole grid inside the container. Values(space-between, space-around, space-evenly, center, start, end)
   align-content: Vertically align the whole grid inside the container. Values(center, space-between, space-evenly, space-around, start, end)


  grid-auto-flow: default value is row, grid-auto-flow: column; grid-template-rows: 100px 200px 100px; Row has been increrase more so, grid-auto-rows: 200px;

  Spanning:
   grid-column-start
   gird-column-end
   grid-colum(shorthand property)
   grid-row-start
   grid-row-end
   grid-row(shorthand property)

   grid-template-areas:
   grid-column-column: repeat(), minmax(), auto-fit(it fitting have the content), auto-fill(it gave space for content)

===============================Animations and Effects=======================================================================

    Filter Property: The filter property defines visual effects to an element.
     Demo : https://codepen.io/stoumann/pen/MWeNmyb

     1.blur(1px)
     2.greyScale(0% - 100%)
     3.brightness(200%)
     4.contrast(0 - 3)
     5.hue-rotate(0 to 360 deg)
     6.invert(0% - 100%)
     7.saturate(0%(completely un-saturated) - 100%(Original Image))
     8.sepia(0%(original Image) - 100%) Note: Negative Values are not allowed
     9.opacity(0 - 1)
     10.dropShadow(horizontal, vertical, blur, color)
     11.url()
     12.none - Default Value


  CSS Gradient:
   1.Linear Gradient(goes down/up/left/right/diagonally)
   2.Conic Gradient(rotated around a center point)
   3.Radial Gradient(defined by their center)

Rule:
 Atleast need two color stops

 Syntax for linear gradient:
   background-image: linear-gradient(direction, color stop1, color stop2, ....)
   Eg:background-image: linear-gradient(red, yellow);
   left to right: linear-ggradient(to right, red, yellow) Values(to right, to left, to bottom, to top)
   Direction diagonally: to bottom right, color1, color2
   we can use angle also

 Syntax for Radial gradient:
   By default shape is ellipse, positon is center.
   background-image: radial-gradient(shape size at position, start-color, ..., last-color);
   Eg: background-image: radial-gradient(red, yellow, green);
   
 Syntax for conic gradient:
  background-image: conic-gradient([from angle] [at position,] color [degree], color [degree], ...);
   background-image: conic-gradient(red 45deg, yellow 90deg, green 210deg);
   Eg: background-image: conic-gradient(red 0deg, red 90deg, yellow 90deg, yellow 180deg, green 180deg, green 270deg, blue 270deg);



     Animations:

     2Dimensional Transform:
      Methods:
       1.translate()
       2.rotate()
       3.scaleX()
       4.scaleY()
       5.skewX()
       6.skewY()
       


       rotate - degree 0 - 360deg
       scale - width, height ...Eg: scale(2, 3)  -  two times of its original width, and three times of its original height: 
       scaleX(2)- 2 times of original width
       scale(Y2)- 2 time of original height
        skew(20deg, 30deg)  /* 20 degress x axix , 30 degress y axis */

      CSS 3D Transforms Methods:
       1.rotateX()
       2.rotateY()
       3.rotateZ()


       CSS Transition:
        transition
        transition-delay - 5s(after 5s only it willl happen)
        transition-duration - 2s, 3s, 5s, ...
        transition-property - background-color, width,...all
        transition-timing-function(ease-in, ease-out, ease-in-out, )
          ease-in = start with slow end with speend
          ease-out - start with speed end with slow
          ease-in-out - combination of ease-in and ease-out
          linear - smoothy normal way

      Animation:
       animation-name:
       animation-duration:

===================================================================================================================================



-->
