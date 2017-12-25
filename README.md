# Classmate
Write less and develop faster with Classmate, an easy to use mobile responsive CSS Utility Library

Installation

To start using Classmate, download the source files and place them in your project css folder, then add a stylesheet <link> in the <head> of your document as shown below.
Please Note: Classmate must be placed last, after all other stylesheets load.

<link rel="stylesheet" href="/css/bootstrap.min.css">
<link rel="stylesheet" href="/css/my-custom-styles.css">
<link rel="stylesheet" href="/css/classmate.1.0.0.min.css">

How It Works

Classmate is a utility library of classes for applying powerful responsive styling to your project, such as padding, margins, font sizes, colors, borders and more.

The Classmate library uses a simple rule for you to follow when applying it's classes, "Model", "Component", "Device", "Value".

    Model - the elements object such as it's padding, margin, border, text, font etc.
    Component - the elements models component such as the position, alignment, weight radius & size.
    Device - the target screen size, seperated with hyphens (-), -xs-, -sm-, -md-, -lg-.
    *Value - the value is how much of the model and/or component you wish to apply, 20px (pixels), 20pct (%), 2em (multiply).

*Classmate applies values in pixels by default. For example, padding20 will apply a 20 pixel padding around the element.
To specify an amount in a value other than pixels, Classmate uses: pct = %, em = multiply (font size only)

Here are some basic lessons to get you on your way with Classmate.

Padding

There are five padding tiers to the Classmate system, one for each range of devices generally support plus an overrule class. Each tier begins with the minimum viewport size and automatically applies the styles to the respective device unless overridden or using an overrule* class.

There are 24 padding sizes in pixels and 8 as a percentage, available with the Classmate library which are as follows:

Padding sizes in pixels (responsive selectors available with this model):
none, 1px, 2px, 3px, 5px, 10px, 15px, 20px, 25px, 30px, 35px, 40px, 45px, 50px, 55px, 60px, 65px, 70px, 75px, 80px, 85px, 90px, 95px, 100px

Padding sizes as a percentage (responsive selectors available with this model):
1%, 2%, 3%, 5%,10%, 15%, 20%, 25%

The padding in the box below will adjust (pixels) depending on your screen size.

HTML Example:
<div class="padding-xs-20 padding-sm-30 padding-md-40 padding-lg-50">Responsive Padding</div>

Being Particular

You can apply padding to individual edges to further customise your elements. For this, the Classmate library uses a simple rule for you to follow when applying classes, "Model", "Component", "Device", "Value". Firstly we will select the model, in this case "padding", then we select the particular component we want to style, for this demonstration we will select the "left" side of our container, so in css terms that's "padding-left". To keep the length of our classes to an understandable minimum, Classmate joins the "model" & "component" names together with the first letter of the second word adopting a capital letter. We then simply select the device size and value seperated with hyphens.

The box below demonstrates a "Left Padding" applied and adjusted for each range of device.

HTML Example:
<div class="paddingLeft-xs-20 paddingLeft-sm-30 paddingLeft-md-40 paddingLeft-lg-50">Responsive Padding Left</div>

Two by Two

To apply padding to either the top and bottom or the left and right edges of an element we use Classmates "Lateral" (top/bottom) & "Gutter" (left/right) names, demonstrated below.

To apply specific sizes of gutter or lateral padding to different devices, we simply apply the device size and and value for example: paddingGutter-xs-10

HTML Example:
<div class="paddingLateral20">20px padding applied to both the top and bottom edges</div>

<div class="paddingGutter20">20px padding applied to both the left and right edges</div>

Overruled

*You can use a non-responsive overrule class to override any padding class in your css. To use an overrule class simply emit the device size you wish to target from the class name as shown below. Note: All hyphens are emitted and for zero padding, the first letter of the second word adopts a capital letter.

HTML Example:
<div class="paddingNone">0px padding on all devices</div>
<div class="padding10">10px padding on all devices</div>


Margin

There are five margin tiers to the Classmate system just like the padding model, one for each range of device plus an overrule class.

There are 24 margin sizes (in pixels) available within the Classmate library which are as follows:

Margin sizes (responsive selectors available with this model):
none, 1px, 2px, 3px, 5px, 10px, 15px, 20px, 25px, 30px, 35px, 40px, 45px, 50px, 55px, 60px, 65px, 70px, 75px, 80px, 85px, 90px, 95px, 100px

HTML Example:
<div class="margin-xs-20 margin-sm-30 margin-md-40 margin-lg-50">Responsive Margin</div>

Being Particular

As with padding, you can apply margins to individual edges to further customise your elements.

HTML Example:
<div class="marginLeft-xs-20 marginLeft-sm-30 marginLeft-md-40 marginLeft-lg-50">Responsive Margin Left</div>

Two by Two

To apply a margin to either the top and bottom or the left and right edges of an element we use Classmates "Lateral" (top/bottom) & "Gutter" (left/right) names, demonstrated below.

To apply specific sizes of gutter or lateral margins to different devices, we simply apply the device size and and value for example: marginGutter-xs-10

HTML Example:
<div class="marginLateral20">20px margin applied to both the top and bottom edges</div>

<div class="marginGutter20">20px margin applied to both the left and right edges</div>

Over The Edge

The Classmate system allows for margins to be stretched beyond their boundries, so to speak!
To expand margins beyond their bounding parent element, we simply apply the action "pull".

HTML Example:
<div class="marginLateral-xs-pull-10 marginLateral-sm-pull-20 marginLateral-md-pull-40 marginLateral-lg-pull-50">Mobile responsive lateral margin pull</div>

<div class="marginRight-xs-pull-10 marginRight-sm-pull-20 marginRight-md-pull-30 marginRight-lg-pull-40">Mobile responsive margin pulled right</div>

Overruled

*You can use a non-responsive overrule class to override any margin class in your css. To use an overrule class simply emit the device size you wish to target from the class name as shown below. Note: All hyphens are emitted and for zero margin, the first letter of the second word adopts a capital letter.

HTML Example:
<div class="marginNone">0px padding on all devices</div>
0px padding on all devices

<div class="margin10">10px padding on all devices</div>
10px padding on all devices

Color

Choose from 109 color variations available with the Classmate color library to use with your backgrounds, buttons, text or vector graphics.

    To apply a color to a background, place the letters "bg" in front of the color name

    <div class="bgWhite">A white background</div>

    To apply color to text, write "color" in front of the color name
    <p class="colorPurple">Purple text</p>

    To fill an element such as an svg, write "fill" in front of the color name

    <svg class="fillOrange">An orange filled vector graphic</svg>

When applying a background color to a link with a "btn" class included, Classmate will automatically apply a hover state to the link.

Example:
<a href="#" class="btn bgPink colorWhite">My Pink Button</a>

The Classmate Color Library
Black
Black1
Black2
Black3
Black4
Black5
Grey1
Grey2
Grey3
Grey4
Grey5
Grey6
Grey7
Grey8
Grey9
BluestoneLight
Bluestone
BluestoneDark
NavyLight
Navy
NavyDark
IndigoLight
Indigo
IndigoDark
ImperialLight
Imperial
ImperialDark
BlueLight
Blue
BlueDark
OceanLight
Ocean
OceanDark
CyanLight
Cyan
CyanDark
CockatooLight
Cockatoo
CockatooDark
TealLight
Teal
TealDark
SpruceLight
Spruce
SpruceDark
GreenLight
Green
GreenDark
GoldenLight
Golden
GoldenDark
CurryLight
Curry
CurryDark
ToastLight
Toast
ToastDark
ButterumLight
Butterum
ButterumDark
OtterLight
Otter
OtterDark
BrownLight
Brown
BrownDark
PortLight
Port
PortDark
LilacLight
Lilac
LilacDark
PurpleLight
Purple
PurpleDark
PinkLight
Pink
PinkDark
PrimroseLight
Primrose
PrimroseDark
GrenadineLight
Grenadine
GrenadineDark
RedLight
Red
RedDark
OrangeLight
Orange
OrangeDark
MapleLight
Maple
MapleDark
PoppyLight
Poppy
PoppyDark
ApricotLight
Apricot
ApricotDark
OliveLight
Olive
OliveDark
VibrantYellowLight
VibrantYellow
VibrantYellowDark
YellowLight
Yellow
YellowDark

Border

Using the Classmate color library you can apply borders to your elements with ease.

HTML Example:
<div class="borderBlack">borderBlack</div>
borderBlack
borderBlack1
borderBlack2
borderBlack3
borderBlack4
borderBlack5
borderGrey1
borderGrey2
borderGrey3
borderGrey4
borderGrey5
borderGrey6
borderGrey7
borderGrey8
borderGrey9
borderBluestoneLight
borderBluestone
borderBluestoneDark
borderNavyLight
borderNavy
borderNavyDark
borderIndigoLight
borderIndigo
borderIndigoDark
borderImperialLight
borderImperial
borderImperialDark
borderSpruceLight
borderSpruce
borderSpruceDark
borderOceanLight
borderOcean
borderOceanDark
borderCyanLight
borderCyan
borderCyanDark
borderBlueLight
borderBlue
borderBlueDark
borderCockatooLight
borderCockatoo
borderCockatooDark
borderTealLight
borderTeal
borderTealDark
borderRedLight
borderRed
borderRedDark
borderGrenadineLight
borderGrenadine
borderGrenadineDark
borderPoppyLight
borderPoppy
borderPoppyDark
borderOrangeLight
borderOrange
borderOrangeDark
borderApricotLight
borderApricot
borderApricotDark
borderToastLight
borderToast
borderToastDark
borderButterumLight
borderButterum
borderButterumDark
borderMapleLight
borderMaple
borderMapleDark
borderBrownLight
borderBrown
borderBrownDark
borderGoldenLight
borderGolden
borderGoldenDark
borderCurryLight
borderCurry
borderCurryDark
borderGreenLight
borderGreen
borderGreenDark
borderVibrantYellowLight
borderVibrantYellow
borderVibrantYellowDark
borderYellowLight
borderYellow
borderYellowDark
borderOliveLight
borderOlive
borderOliveDark
borderPrimroseLight
borderPrimrose
borderPrimroseDark
borderPinkLight
borderPink
borderPinkDark
borderLilacLight
borderLilac
borderLilacDark
borderPurpleLight
borderPurple
borderPurpleDark
borderOtterLight
borderOtter
borderOtterDark
borderPortLight
borderPort
borderPortDark
borderWhite

Being Particular

Go ahead and customise your elements by adding colored borders to any given edge of an element.

HTML Example:
<div class="borderRightPink">borderRightPink</div>

Mix It Up

HTML Example:
<div class="borderLeftOrange borderTopBlue borderRightGreen borderBottomPurple">go wild, create border combinations!</div>

Note: There are also borderTransparent & borderNone classes available in all edges and screen sizes.

Two by Two

Sometimes it's necessary to add borders to both the top and bottom or the left and right edges of an element. Classmates "Lateral" (top/bottom) & "Gutter" (left/right) names, are also available for the border model.

HTML Example:
<div class="borderLateralBlack3">borderLateralBlack3</div>
borderLateralBlack3

<div class="borderGutterGrey5">borderGutterGrey5</div>

Give It Some Style

Classmate has included 3 border styles to choose from and can be styled with any color available from the Classmate color library.

HTML Example:
<div class="borderBottomPink">borderBottomPink</div>
borderBottomPink

<div class="borderDashedBottomBlue">borderDashedBottomBlue</div>

<div class="borderDottedBottomGreen">borderDottedBottomGreen</div>

Let's Round It Off

Included in the Classmate border model are several variations of border radius allowing you to apply an equal amount of border radius to all four corners, or customise each corner individually.

Border radius' can be applied in the following pixel values: none, 5, 6, 7, 8, 9, 10, 12, 15, 20 & 25

HTML Example:
<div class="borderRadius10">borderRadius10</div>
borderRadius10
borderRadius-tl-5
borderRadius-tltr-6
borderRadius-tlbr-7
borderRadius-tr-8
borderRadius-trbr-9
borderRadius-trbl-10
borderRadius-br-12
borderRadius-brbl-15
borderRadius-bl-20
borderRadius-bltl-25
borderRadiusNone

Need a circle? no problem, just use the circle class and voila!

HTML Example:
<div class="circle padding15 bgGreenDark colorWhite"><i class="fa fa-check fontSize20px"></i></div>

Font

Within the Classmate font model we can adjust the size to respond to different devices, increase or decrease the weight and even change the style of your fonts all from your HTML.

Classmate has 3 mobile responsive font measurements to adjust your fonts with.
Pixels (px)

Pixel sizes (responsive selectors available with this model):
10px, 11px, 12px, 14px, 16px, 18px, 20px, 22px, 24px, 26px, 28px, 30px, 32px, 34px, 36px, 38px, 40px, 42px, 44px, 46px, 48px, 50px, 60px, 70px, 80px, 90px, 100px

HTML Example:
<span class="fontSize20px">Font size 20px</span>


Multiply (em)

Multiplied sizes (responsive selectors available with this model):
06em, 07em, 08em, 1em, 11em, 12em, 13em, 15em, 16em, 17em, 18em, 2em, 25em, 3em, 35em, 4em, 45em, 5em

HTML Example:
<span class="fontSize2em">Font size 2em</span>


Percent (pct)

Percentage sizes (responsive selectors available with this model):
10pct, 20pct, 30pct, 40pct, 50pct, 60pct, 70pct, 80pct, 90pct, 100pct, 110pct, 120pct, 130pct, 140pct, 150pct, 160pct, 170pct, 180pct, 190pct, 200pct, 300pct, 400pct, 500pct, 600pct, 700pct, 800pct, 900pct, 1000pct

HTML Example:
<span class="fontSize200pct">Font size 200%</span>


Make It Responsive

Use the device selectors to make your font sizes responsive!

HTML Example:
<span class="fontSize-xs-12px fontSize-sm-14px fontSize-md-16px fontSize-lg-20px">Mobile responsive font size (px)</span>

Give It Some Weight

To increase or decrease the weight of your text, the Classmate library has provided a selection of font weights for you to choose from.

Font weights (responsive selectors available with this model):
fontWeight + Normal, Bold, Bolder, Lighter, 100, 200, 300, 400, 500, 600, 700, 800, 900

HTML Example:
<span class="fontWeight600">fontWeight600</span>


Text

Within the Classmate text model we can adjust the alignment and transform it to respond to different devices.
Alignment

Text alignments (responsive selectors available with this model):
textLeft, textRight, textCenter, textJustify, textStart, textEnd

HTML Example:
<span class="text-xs-center text-md-left">Responsive text alignment</span>

Overruled

You can use a non-responsive overrule class to override any text alignment set in your css. To use an overrule class simply emit the device size you wish to target from the class name as shown below.

HTML Example:
<div class="textCenter">Text is centered on all devices</div>

Under or Over

Need to underline your text? Apply Classmates textUnderline to your text and you're done.

Text decoration (responsive selectors available with this model):
textUnderline, textOverline, textLineThrough

HTML Example:
<div class="textUnderline">Text is underlined</div>
<div class="textLineThrough">Text has a line through it</div>


Wrap It Up

To make mobile responsiveness even better, Classmate has included a wrap component to its text model library.

Wrap options available:
textWrapNone, textWrapNormal, wordBreakNormal, wordBreakAll, wordKeepAll

HTML Example:
<div class="width250 wordBreakAll">TheTextWillBreakTheWordToFitTheBoundingBox - TheBoundingBoxHasAFixedWidthOf250Pixels</div>

Display

Classmates display model makes it easy to display or hide elements as block, inline, table, cell or flex content.

Display options available:
displayNone, displayBlock, displayInlineBlock, displayTable, displayTableCell, displayFlexbox

HTML Example:
<span class="displayBlock">HTML span element displayed as a block</span>

<div class="displayInlineBlock">HTML div element displayed inline</div>

Float

Floating elements on your page to the left, right or center with Classmate couldn't be easier.

Float options (responsive selectors available with this model):
floatLeft, floatRight, floatCenter

HTML Example:
<div class="floatLeft">HTML element floated left</div>

Make it Responsive

Classmates float model is also mobile responsive.

Once again just tell Classmate which screen size you wish to float you elements for and you're good to go!

HTML Example:
<div class="float-xs-center float-md-left">This element will float left for desktops, and centered for smaller devices</div>

Vertical

Vertically aligning text, images or components within tables on your page with Classmate couldn't be easier. Classmate can even center an element without any tables or JavaScript required.

Vertical options available:
verticalTop, verticalMiddle, verticalCenter**, verticalBottom, verticalBaseline, verticalSub, verticalSuper

**The Classmate library includes a unique component to vertically align any element on a page, Classmate calls this "verticalCenter".

To use Classmates verticalCenter component, simply wrap any height defined verticalCenter element around another element with a class name of container or container-fluid (as shown below).

HTML Example:
<div class="verticalCenter height200 borderGrey8"><div class="container">This text is vertically aligned in the middle</div></div>

Position

The Classmate library contains 4 of the most commonly used element positions to utilise with your project.

Position options available:
positionFixed, positionAbsolute, positionRelative, positionStatic

Of course when applying a position to your element you may wish to define it placement. For this Classmate uses Top, Right, Bottom, Left, so you can now tell your element exactly where it should be displayed.

There are 40 position placements in pixels and 13 as a percentage, available with the Classmate library which are as follows:

Position placements in pixels (responsive selectors available with this model):
none, 1px, 2px, 3px, 5px, 10px, 15px, 20px, 25px, 30px, 35px, 40px, 45px, 50px, 55px, 60px, 65px, 70px, 75px, 80px, 85px, 90px, 95px, 100px, 110px, 120px, 130px, 140px, 150px, 160px, 170px, 180px, 190px, 200px, 250px, 300px, 350px, 400px, 450px, 500px

Position placements as a percentage (responsive selectors available with this model):
1%, 2%, 3%, 5%,10%, 15%, 20%, 25%, 30%, 35%, 40%, 45%, 50%

HTML Example:
<div class="positionRelative height200 borderGrey8"><div class="positionAbsolute positionTop50 positionRight100">This text is positioned 50px from the top, 100px from the right</div></div>

Width

The Classmate width model uses 3 measurement scales to select the width of your element, pixels (px), percentage (pct) and viewport (vw)

There are 43 width options in pixels, 15 as a percentage and 13 as viewport width measurments available with the Classmate library which are as follows:

Width options in pixels:
5px, 10px, 15px, 20px, 25px, 30px, 40px, 50px, 60px, 70px, 75px, 80px, 90px, 100px, 125px, 150px, 175px, 200px, 225px, 250px, 275px, 300px, 325px, 350px, 375px, 400px, 425px, 450px, 475px, 500px, 525px, 550px, 575px, 600px, 650px, 700px, 750px, 800px, 850px, 900px, 950px, 1000px

Width options as a percentage:
10%, 12%, 15%, 17%, 20%, 25%, 30%, 33%, 50%, 60%, 66%, 70%, 75%, 80%, 90%, 100%

Width options in viewport width:
10vw, 15vw, 20vw, 25vw, 30vw, 33vw, 40vw, 50vw, 60vw, 66vw, 70vw, 75vw, 80vw, 90vw, 100vw

HTML Example:
<div class="width25pct">Element is 25% the width of it's parent container</div>

Height

The Classmate height model uses 3 measurement scales to select the height of your element, pixels (px), percentage (pct) and viewport (vh)

There are 34 height options in pixels, 14 as a percentage and 13 as viewport height measurments available with the Classmate library which are as follows:

Height options in pixels:
5px, 10px, 15px, 20px, 25px, 30px, 40px, 50px, 60px, 70px, 80px, 90px, 100px, 125px, 130px, 150px, 175px, 200px, 225px, 250px, 275px, 300px, 325px, 350px, 375px, 400px, 425px, 450px, 475px, 500px, 525px, 550px, 575px, 600px

Height options as a percentage:
10%, 15%, 20%, 25%, 30%, 33%, 40%, 50%, 60%, 66%, 70%, 75%, 80%, 90%, 100%

Height options in viewport width:
10vw, 15vw, 20vw, 25vw, 30vw, 33vw, 40vw, 50vw, 60vw, 66vw, 70vw, 75vw, 80vw, 90vw, 100vw

HTML Example:
<div class="height100">Element is 100px high</div>

Overflow

Within the Classmate overflow model you can add and remove scrollbars from elements.

Overflow options available:
overflowAuto, overflowHidden, overflowScroll, overflowVisible, overflowNoContent, overflowNoDisplay, overflowAuto-x, overflowHidden-x, overflowScroll-x, overflowVisible-x, overflowNoContent-x, overflowNoDisplay-x, overflowAuto-y, overflowHidden-y, overflowScroll-y, overflowVisible-y, overflowNoContent-y, overflowNoDisplay-y, overflowWrapNormal, overflowWrapBreak

HTML Example:
<div class="overflowScroll-x">Element with a horizontal scrollbar</div>

<div class="overflowScroll-y">Element with a vertical scrollbar</div>


Clear

Clearing elements on your page from the left or right with Classmates clear model is another handy feature!

Clear options (responsive selectors available with this model):
clearNone, clearLeft, clearRight, clearBoth, clearBlock

HTML Example:
<div class="clearBlock">clearBlock completely clears and shifts to a new line and creates a block element</div>
