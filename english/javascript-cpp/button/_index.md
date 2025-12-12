---
title: Button
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents the Forms control Button
type: docs
url: /javascript-cpp/button/
---

## Button class

Represents the Forms control: Button

```javascript
class Button extends Shape;
```


### Example
```javascript
const { Workbook, MsoDrawingType, Color, PlacementType, SaveFormat } = AsposeCells;

//Create a new Workbook.
var workbook = new Workbook();
//Get the first worksheet in the workbook.
var sheet = workbook.worksheets.get(0);

//Add a new button to the worksheet.
var button = sheet.shapes.addShape(MsoDrawingType.Button, 2, 0, 2, 0, 28, 80);
//Set the caption of the button.
button.text = "Aspose";
//Set the Placement Type, the way the
//button is attached to the cells.
button.placement = PlacementType.FreeFloating;
//Set the font name.
button.font.setName("Tahoma");
//Set the caption string bold.
button.font.isBold = true;
//Set the color to blue.
button.font.color = Color.Blue;
//Set the hyperlink for the button.
button.addHyperlink("http://www.aspose.com/");

//Saves the file.
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Constructors

| Name | Description |
| --- | --- |
| [constructor(Shape)](#constructor-shape-)| Constructs from a parent object convertible to this. |

## Properties

| Property | Type | Description |
| --- | --- | --- |
| [macroName](#macroName--)| string | Gets and sets the name of macro. |
| [isEquation](#isEquation--)| boolean | Readonly. Indicates whether the shape only contains an equation. |
| [isSmartArt](#isSmartArt--)| boolean | Readonly. Indicates whether the shape is a smart art. |
| [zOrderPosition](#zOrderPosition--)| number | Returns the position of a shape in the z-order. |
| [name](#name--)| string | Gets and sets the name of the shape. |
| [alternativeText](#alternativeText--)| string | Returns or sets the descriptive (alternative) text string of the [Shape](../shape/) object. |
| [title](#title--)| string | Specifies the title (caption) of the current shape object. |
| [line](#line--)| LineFormat | Readonly. Gets line style |
| [fill](#fill--)| FillFormat | Readonly. Returns a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified shape. |
| [shadowEffect](#shadowEffect--)| ShadowEffect | Readonly. Represents a [Drawing.ShadowEffect](../drawing.shadoweffect/) object that specifies shadow effect for the chart element or shape. |
| [reflection](#reflection--)| ReflectionEffect | Readonly. Represents a [ReflectionEffect](../reflectioneffect/) object that specifies reflection effect for the chart element or shape. |
| [glow](#glow--)| GlowEffect | Readonly. Represents a [GlowEffect](../gloweffect/) object that specifies glow effect for the chart element or shape. |
| [softEdges](#softEdges--)| number | Gets and sets the radius of blur to apply to the edges, in unit of points. |
| [threeDFormat](#threeDFormat--)| ThreeDFormat | Readonly. Gets and sets 3d format of the shape. |
| [formatPicture](#formatPicture--)| MsoFormatPicture | Readonly. Gets and sets the options of the picture format. |
| [isHidden](#isHidden--)| boolean | Indicates whether the object is visible. |
| [isLockAspectRatio](#isLockAspectRatio--)| boolean | True means that aspect ratio of the shape is locked. |
| [isAspectRatioLocked](#isAspectRatioLocked--)| boolean | True means that aspect ratio of the shape is locked. |
| [rotationAngle](#rotationAngle--)| number | Gets and sets the rotation of the shape. |
| [hyperlink](#hyperlink--)| Hyperlink | Readonly. Gets the hyperlink of the shape. |
| [id](#id--)| number | Readonly. Gets the identifier of this shape. |
| [spid](#spid--)| string | Readonly. Specifies an optional string identifier that an application can use to identify the particular shape. |
| [spt](#spt--)| number | Readonly. Specifies an optional number that an application can use to associate the particular shape with a defined shape type. |
| [worksheet](#worksheet--)| Worksheet | Readonly. Gets the [Worksheet](../worksheet/) object which contains this shape. |
| [isGroup](#isGroup--)| boolean | Readonly. Indicates whether this shape is a group shape. |
| [isInGroup](#isInGroup--)| boolean | Readonly. Indicates whether the shape is grouped. |
| [isWordArt](#isWordArt--)| boolean | Readonly. Indicates whether this shape is a word art. |
| [textEffect](#textEffect--)| TextEffectFormat | Readonly. Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape. Applies to Shape objects that represent WordArt. |
| [isLocked](#isLocked--)| boolean | True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected. |
| [isPrintable](#isPrintable--)| boolean | Indicates whether the object is printable. If False, this shape will not be printed when printing. |
| [msoDrawingType](#msoDrawingType--)| MsoDrawingType | Readonly. Gets drawing type. |
| [autoShapeType](#autoShapeType--)| AutoShapeType | Gets and sets the auto shape type. |
| [anchorType](#anchorType--)| ShapeAnchorType | Gets and set the type of the shape anchor placeholder. |
| [placement](#placement--)| PlacementType | Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. |
| [upperLeftRow](#upperLeftRow--)| number | Represents the top row index. |
| [upperDeltaY](#upperDeltaY--)| number | Gets or sets the shape's vertical offset from its upper left corner row. |
| [upperLeftColumn](#upperLeftColumn--)| number | Represents upper left corner column index. |
| [upperDeltaX](#upperDeltaX--)| number | Gets or sets the shape's horizontal offset from its upper left corner column. |
| [lowerRightRow](#lowerRightRow--)| number | Represents lower right corner row index. |
| [lowerDeltaY](#lowerDeltaY--)| number | Gets or sets the shape's vertical offset from its lower right corner row. |
| [lowerRightColumn](#lowerRightColumn--)| number | Represents lower right corner column index. |
| [lowerDeltaX](#lowerDeltaX--)| number | Gets or sets the shape's horizontal  offset from its lower right corner column. |
| [right](#right--)| number | Represents the width of the shape's horizontal  offset from its lower right corner column, in unit of pixels. |
| [bottom](#bottom--)| number | Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels. |
| [width](#width--)| number | Represents the width of shape, in unit of pixels. |
| [widthInch](#widthInch--)| number | Represents the width of the shape, in unit of inch. |
| [widthPt](#widthPt--)| number | Represents the width of the shape, in unit of point. |
| [widthCM](#widthCM--)| number | Represents the width of the shape, in unit of centimeters. |
| [height](#height--)| number | Represents the height of shape, in unit of pixel. |
| [heightInch](#heightInch--)| number | Represents the height of the shape, in unit of inches. |
| [heightPt](#heightPt--)| number | Represents the height of the shape, in unit of points. |
| [heightCM](#heightCM--)| number | Represents the height of the shape, in unit of centimeters. |
| [left](#left--)| number | Represents the horizontal offset of shape from its left column, in unit of pixels. |
| [leftInch](#leftInch--)| number | Represents the horizontal offset of shape from its left column, in unit of inches. |
| [leftCM](#leftCM--)| number | Represents the horizontal offset of shape from its left column, in unit of centimeters. |
| [top](#top--)| number | Represents the vertical offset of shape from its top row, in unit of pixels. |
| [topInch](#topInch--)| number | Represents the vertical offset of shape from its top row, in unit of inches. |
| [topCM](#topCM--)| number | Represents the vertical offset of shape from its top row, in unit of centimeters. |
| [topToCorner](#topToCorner--)| number | Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels. |
| [leftToCorner](#leftToCorner--)| number | Gets and sets the horizonal offset of shape from worksheet left border. |
| [x](#x--)| number | Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels. |
| [y](#y--)| number | Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels. |
| [widthScale](#widthScale--)| number | Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100; |
| [heightScale](#heightScale--)| number | Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100; |
| [topInShape](#topInShape--)| number | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. |
| [leftInShape](#leftInShape--)| number | Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. |
| [widthInShape](#widthInShape--)| number | Represents the width of the shape, in unit of 1/4000 of the parent shape. |
| [heightInShape](#heightInShape--)| number | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. |
| [group](#group--)| GroupShape | Readonly. Gets the group shape which contains this shape. |
| [type](#type--)| AutoShapeType | Readonly. Gets the auto shape type. |
| [hasLine](#hasLine--)| boolean | Gets and sets the line border of the shape is visible. |
| [isFilled](#isFilled--)| boolean | Indicates whether the fill format is visible. |
| [isFlippedHorizontally](#isFlippedHorizontally--)| boolean | Gets and sets whether shape is horizontally flipped . |
| [isFlippedVertically](#isFlippedVertically--)| boolean | Gets and sets whether shape is vertically flipped . |
| [actualLowerRightRow](#actualLowerRightRow--)| number | Readonly. Get the actual bottom row. |
| [relativeToOriginalPictureSize](#relativeToOriginalPictureSize--)| boolean | Indicates whether shape is relative to original picture size. |
| [linkedCell](#linkedCell--)| string | Gets or sets the worksheet range linked to the control's value. |
| [inputRange](#inputRange--)| string | Gets or sets the worksheet range used to fill the specified combo box. |
| [textShapeType](#textShapeType--)| AutoShapeType | Gets and sets the preset text shape type. |
| [textBody](#textBody--)| FontSettingCollection | Readonly. Gets and sets the setting of the shape's text. |
| [font](#font--)| Font | Represents the font of shape. |
| [textOptions](#textOptions--)| TextOptions | Represents the text options of the shape. |
| [text](#text--)| string | Gets and sets the text of this shape. |
| [isRichText](#isRichText--)| boolean | Readonly. Whether or not the text is rich text. |
| [htmlText](#htmlText--)| string | Gets and sets the html string which contains data and some formats in this textbox. |
| [textVerticalOverflow](#textVerticalOverflow--)| TextOverflowType | Gets and sets the text vertical overflow type of the shape which contains text. |
| [textHorizontalOverflow](#textHorizontalOverflow--)| TextOverflowType | Gets and sets the text horizontal overflow type of the shape which contains text. |
| [isTextWrapped](#isTextWrapped--)| boolean | Gets and sets the text wrapped type of the shape which contains text. |
| [textOrientationType](#textOrientationType--)| TextOrientationType | Gets and sets the text orientation type of the shape. |
| [textHorizontalAlignment](#textHorizontalAlignment--)| TextAlignmentType | Gets and sets the text horizontal alignment type of the shape. |
| [textVerticalAlignment](#textVerticalAlignment--)| TextAlignmentType | Gets and sets the text vertical alignment type of the shape. |
| [textDirection](#textDirection--)| TextDirectionType | Gets/Sets the direction of the text flow for this object. |
| [textBoxOptions](#textBoxOptions--)| TextBoxOptions | Readonly. Gets the text information in the shape |
| [controlData](#controlData--)| Uint8Array | Readonly. Gets the data of control. |
| [activeXControl](#activeXControl--)| ActiveXControl | Readonly. Gets the ActiveX control. |
| [paths](#paths--)| ShapePathCollection | Readonly. Gets the paths of a custom geometric shape. |
| [geometry](#geometry--)| Geometry | Readonly. Gets the geometry |
| [isDecorative](#isDecorative--)| boolean | Indicates whether the object is decorative. |

## Methods

| Method | Description |
| --- | --- |
| [toFrontOrBack(number)](#toFrontOrBack-number-)| Brings the shape to the front or sends the shape to back. |
| [getLockedProperty(ShapeLockType)](#getLockedProperty-shapelocktype-)| Gets the value of locked property. |
| [setLockedProperty(ShapeLockType, boolean)](#setLockedProperty-shapelocktype-boolean-)| Set the locked property. |
| [addHyperlink(string)](#addHyperlink-string-)| Adds a hyperlink to the shape. |
| [removeHyperlink()](#removeHyperlink--)| Removes the hyperlink of the shape. |
| [moveToRange(number, number, number, number)](#moveToRange-number-number-number-number-)| Moves the shape to a specified range. |
| [alignTopRightCorner(number, number)](#alignTopRightCorner-number-number-)| Moves the picture to the top-right corner. |
| [getConnectionPoints()](#getConnectionPoints--)| Get the connection points |
| [toImageAsync(ImageType)](#toImageAsync-imagetype-)| Creates the shape image and saves it to a stream in the specified format. |
| [toImageAsync(string, ImageOrPrintOptions)](#toImageAsync-string-imageorprintoptions-)| Saves the shape to a file. |
| [toImageAsync(ImageOrPrintOptions)](#toImageAsync-imageorprintoptions-)| Saves the shape to a stream. |
| [toImage(ImageType)](#toImage-imagetype-)| Creates the shape image and saves it to a stream in the specified format. |
| [toImage(string, ImageOrPrintOptions)](#toImage-string-imageorprintoptions-)| Saves the shape to a file. |
| [toImage(ImageOrPrintOptions)](#toImage-imageorprintoptions-)| Saves the shape to a stream. |
| [getLinkedCell(boolean, boolean)](#getLinkedCell-boolean-boolean-)| Gets the range linked to the control's value. |
| [setLinkedCell(string, boolean, boolean)](#setLinkedCell-string-boolean-boolean-)| Sets the range linked to the control's value. |
| [getInputRange(boolean, boolean)](#getInputRange-boolean-boolean-)| Gets the range used to fill the control. |
| [setInputRange(string, boolean, boolean)](#setInputRange-string-boolean-boolean-)| Sets the range used to fill the control. |
| [updateSelectedValue()](#updateSelectedValue--)| Update the selected value by the value of the linked cell. |
| [calculateTextSize()](#calculateTextSize--)| Recalculate the text area |
| [formatCharacters(number, number, Font, StyleFlag)](#formatCharacters-number-number-font-styleflag-)| Formats some characters with the font setting. |
| [characters(number, number)](#characters-number-number-)| Returns a Characters object that represents a range of characters within the text. |
| [getRichFormattings()](#getRichFormattings--)| Returns all Characters objects that represents a range of characters within the text . |
| [removeActiveXControl()](#removeActiveXControl--)| Remove activeX control. |
| [getActualBox()](#getActualBox--)| Get the actual position and size of the shape (after applying rotation, flip, etc.) |
| [fitToTextSize()](#fitToTextSize--)| Recalculate a text area suitable for displaying all text content. |
| [getResultOfSmartArt()](#getResultOfSmartArt--)| Converting smart art to grouped shapes. |
| [isSameSetting(VObject)](#isSameSetting-vobject-)| Returns whether the shape is same. |


### constructor(Shape) {#constructor-shape-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: Shape);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Shape | The parent object. |

### macroName {#macroName--}

Gets and sets the name of macro.

```javascript
macroName : string;
```


### isEquation {#isEquation--}

Readonly. Indicates whether the shape only contains an equation.

```javascript
isEquation : boolean;
```


### isSmartArt {#isSmartArt--}

Readonly. Indicates whether the shape is a smart art.

```javascript
isSmartArt : boolean;
```


**Remarks**

Only for ooxml file.

### zOrderPosition {#zOrderPosition--}

Returns the position of a shape in the z-order.

```javascript
zOrderPosition : number;
```


### name {#name--}

Gets and sets the name of the shape.

```javascript
name : string;
```


### alternativeText {#alternativeText--}

Returns or sets the descriptive (alternative) text string of the [Shape](../shape/) object.

```javascript
alternativeText : string;
```


### title {#title--}

Specifies the title (caption) of the current shape object.

```javascript
title : string;
```


### line {#line--}

Readonly. Gets line style

```javascript
line : LineFormat;
```


### fill {#fill--}

Readonly. Returns a [FillFormat](../fillformat/) object that contains fill formatting properties for the specified shape.

```javascript
fill : FillFormat;
```


### shadowEffect {#shadowEffect--}

Readonly. Represents a [Drawing.ShadowEffect](../drawing.shadoweffect/) object that specifies shadow effect for the chart element or shape.

```javascript
shadowEffect : ShadowEffect;
```


### reflection {#reflection--}

Readonly. Represents a [ReflectionEffect](../reflectioneffect/) object that specifies reflection effect for the chart element or shape.

```javascript
reflection : ReflectionEffect;
```


### glow {#glow--}

Readonly. Represents a [GlowEffect](../gloweffect/) object that specifies glow effect for the chart element or shape.

```javascript
glow : GlowEffect;
```


### softEdges {#softEdges--}

Gets and sets the radius of blur to apply to the edges, in unit of points.

```javascript
softEdges : number;
```


### threeDFormat {#threeDFormat--}

Readonly. Gets and sets 3d format of the shape.

```javascript
threeDFormat : ThreeDFormat;
```


### formatPicture {#formatPicture--}

Readonly. Gets and sets the options of the picture format.

```javascript
formatPicture : MsoFormatPicture;
```


### isHidden {#isHidden--}

Indicates whether the object is visible.

```javascript
isHidden : boolean;
```


### isLockAspectRatio {#isLockAspectRatio--}

True means that aspect ratio of the shape is locked.

```javascript
isLockAspectRatio : boolean;
```


**Remarks**

Only for pictures and Ole Objects. NOTE: This member is now obsolete. Instead, please use Shape.IsAspectRatioLocked property. This property will be removed 12 months later since July 2024. Aspose apologizes for any inconvenience you may have experienced.

### isAspectRatioLocked {#isAspectRatioLocked--}

True means that aspect ratio of the shape is locked.

```javascript
isAspectRatioLocked : boolean;
```


**Remarks**

Only for pictures and Ole Objects.

### rotationAngle {#rotationAngle--}

Gets and sets the rotation of the shape.

```javascript
rotationAngle : number;
```


### hyperlink {#hyperlink--}

Readonly. Gets the hyperlink of the shape.

```javascript
hyperlink : Hyperlink;
```


### id {#id--}

Readonly. Gets the identifier of this shape.

```javascript
id : number;
```


### spid {#spid--}

Readonly. Specifies an optional string identifier that an application can use to identify the particular shape.

```javascript
spid : string;
```


### spt {#spt--}

Readonly. Specifies an optional number that an application can use to associate the particular shape with a defined shape type.

```javascript
spt : number;
```


### worksheet {#worksheet--}

Readonly. Gets the [Worksheet](../worksheet/) object which contains this shape.

```javascript
worksheet : Worksheet;
```


### isGroup {#isGroup--}

Readonly. Indicates whether this shape is a group shape.

```javascript
isGroup : boolean;
```


### isInGroup {#isInGroup--}

Readonly. Indicates whether the shape is grouped.

```javascript
isInGroup : boolean;
```


### isWordArt {#isWordArt--}

Readonly. Indicates whether this shape is a word art.

```javascript
isWordArt : boolean;
```


**Remarks**

Only for the Legacy Shape of xls file.

### textEffect {#textEffect--}

Readonly. Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape. Applies to Shape objects that represent WordArt.

```javascript
textEffect : TextEffectFormat;
```


### isLocked {#isLocked--}

True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected.

```javascript
isLocked : boolean;
```


### isPrintable {#isPrintable--}

Indicates whether the object is printable. If False, this shape will not be printed when printing.

```javascript
isPrintable : boolean;
```


### msoDrawingType {#msoDrawingType--}

Readonly. Gets drawing type.

```javascript
msoDrawingType : MsoDrawingType;
```


### autoShapeType {#autoShapeType--}

Gets and sets the auto shape type.

```javascript
autoShapeType : AutoShapeType;
```


### anchorType {#anchorType--}

Gets and set the type of the shape anchor placeholder.

```javascript
anchorType : ShapeAnchorType;
```


### placement {#placement--}

Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.

```javascript
placement : PlacementType;
```


### upperLeftRow {#upperLeftRow--}

Represents the top row index.

```javascript
upperLeftRow : number;
```


**Remarks**

If the shape is in the shape or in the group , UpperLeftRow will be ignored.

### upperDeltaY {#upperDeltaY--}

Gets or sets the shape's vertical offset from its upper left corner row.

```javascript
upperDeltaY : number;
```


**Remarks**

The range of value is 0 to 256.

### upperLeftColumn {#upperLeftColumn--}

Represents upper left corner column index.

```javascript
upperLeftColumn : number;
```


### upperDeltaX {#upperDeltaX--}

Gets or sets the shape's horizontal offset from its upper left corner column.

```javascript
upperDeltaX : number;
```


**Remarks**

The range of value is 0 to 1024.

### lowerRightRow {#lowerRightRow--}

Represents lower right corner row index.

```javascript
lowerRightRow : number;
```


### lowerDeltaY {#lowerDeltaY--}

Gets or sets the shape's vertical offset from its lower right corner row.

```javascript
lowerDeltaY : number;
```


**Remarks**

The range of value is 0 to 256.

### lowerRightColumn {#lowerRightColumn--}

Represents lower right corner column index.

```javascript
lowerRightColumn : number;
```


### lowerDeltaX {#lowerDeltaX--}

Gets or sets the shape's horizontal  offset from its lower right corner column.

```javascript
lowerDeltaX : number;
```


**Remarks**

The range of value is 0 to 1024.

### right {#right--}

Represents the width of the shape's horizontal  offset from its lower right corner column, in unit of pixels.

```javascript
right : number;
```


### bottom {#bottom--}

Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels.

```javascript
bottom : number;
```


### width {#width--}

Represents the width of shape, in unit of pixels.

```javascript
width : number;
```


### widthInch {#widthInch--}

Represents the width of the shape, in unit of inch.

```javascript
widthInch : number;
```


### widthPt {#widthPt--}

Represents the width of the shape, in unit of point.

```javascript
widthPt : number;
```


### widthCM {#widthCM--}

Represents the width of the shape, in unit of centimeters.

```javascript
widthCM : number;
```


### height {#height--}

Represents the height of shape, in unit of pixel.

```javascript
height : number;
```


### heightInch {#heightInch--}

Represents the height of the shape, in unit of inches.

```javascript
heightInch : number;
```


### heightPt {#heightPt--}

Represents the height of the shape, in unit of points.

```javascript
heightPt : number;
```


### heightCM {#heightCM--}

Represents the height of the shape, in unit of centimeters.

```javascript
heightCM : number;
```


### left {#left--}

Represents the horizontal offset of shape from its left column, in unit of pixels.

```javascript
left : number;
```


### leftInch {#leftInch--}

Represents the horizontal offset of shape from its left column, in unit of inches.

```javascript
leftInch : number;
```


### leftCM {#leftCM--}

Represents the horizontal offset of shape from its left column, in unit of centimeters.

```javascript
leftCM : number;
```


### top {#top--}

Represents the vertical offset of shape from its top row, in unit of pixels.

```javascript
top : number;
```


**Remarks**

If the shape is in the chart, represents the vertical offset of shape from its top border.

### topInch {#topInch--}

Represents the vertical offset of shape from its top row, in unit of inches.

```javascript
topInch : number;
```


### topCM {#topCM--}

Represents the vertical offset of shape from its top row, in unit of centimeters.

```javascript
topCM : number;
```


### topToCorner {#topToCorner--}

Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels.

```javascript
topToCorner : number;
```


### leftToCorner {#leftToCorner--}

Gets and sets the horizonal offset of shape from worksheet left border.

```javascript
leftToCorner : number;
```


### x {#x--}

Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels.

```javascript
x : number;
```


### y {#y--}

Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels.

```javascript
y : number;
```


### widthScale {#widthScale--}

Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100;

```javascript
widthScale : number;
```


### heightScale {#heightScale--}

Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100;

```javascript
heightScale : number;
```


### topInShape {#topInShape--}

Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.

```javascript
topInShape : number;
```


**Remarks**

Only Applies when this shape in the group or chart.

### leftInShape {#leftInShape--}

Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape.

```javascript
leftInShape : number;
```


**Remarks**

Only Applies when this shape in the group or chart.

### widthInShape {#widthInShape--}

Represents the width of the shape, in unit of 1/4000 of the parent shape.

```javascript
widthInShape : number;
```


**Remarks**

Only Applies when this shape in the group or chart.

### heightInShape {#heightInShape--}

Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape..

```javascript
heightInShape : number;
```


**Remarks**

Only Applies when this shape in the group or chart.

### group {#group--}

Readonly. Gets the group shape which contains this shape.

```javascript
group : GroupShape;
```


### type {#type--}

Readonly. Gets the auto shape type.

```javascript
type : AutoShapeType;
```


### hasLine {#hasLine--}

Gets and sets the line border of the shape is visible.

```javascript
hasLine : boolean;
```


### isFilled {#isFilled--}

Indicates whether the fill format is visible.

```javascript
isFilled : boolean;
```


### isFlippedHorizontally {#isFlippedHorizontally--}

Gets and sets whether shape is horizontally flipped .

```javascript
isFlippedHorizontally : boolean;
```


### isFlippedVertically {#isFlippedVertically--}

Gets and sets whether shape is vertically flipped .

```javascript
isFlippedVertically : boolean;
```


### actualLowerRightRow {#actualLowerRightRow--}

Readonly. Get the actual bottom row.

```javascript
actualLowerRightRow : number;
```


### relativeToOriginalPictureSize {#relativeToOriginalPictureSize--}

Indicates whether shape is relative to original picture size.

```javascript
relativeToOriginalPictureSize : boolean;
```


### linkedCell {#linkedCell--}

Gets or sets the worksheet range linked to the control's value.

```javascript
linkedCell : string;
```


### inputRange {#inputRange--}

Gets or sets the worksheet range used to fill the specified combo box.

```javascript
inputRange : string;
```


### textShapeType {#textShapeType--}

Gets and sets the preset text shape type.

```javascript
textShapeType : AutoShapeType;
```


### textBody {#textBody--}

Readonly. Gets and sets the setting of the shape's text.

```javascript
textBody : FontSettingCollection;
```


### font {#font--}

Represents the font of shape.

```javascript
font : Font;
```


### textOptions {#textOptions--}

Represents the text options of the shape.

```javascript
textOptions : TextOptions;
```


### text {#text--}

Gets and sets the text of this shape.

```javascript
text : string;
```


### isRichText {#isRichText--}

Readonly. Whether or not the text is rich text.

```javascript
isRichText : boolean;
```


### htmlText {#htmlText--}

Gets and sets the html string which contains data and some formats in this textbox.

```javascript
htmlText : string;
```


### textVerticalOverflow {#textVerticalOverflow--}

Gets and sets the text vertical overflow type of the shape which contains text.

```javascript
textVerticalOverflow : TextOverflowType;
```


### textHorizontalOverflow {#textHorizontalOverflow--}

Gets and sets the text horizontal overflow type of the shape which contains text.

```javascript
textHorizontalOverflow : TextOverflowType;
```


### isTextWrapped {#isTextWrapped--}

Gets and sets the text wrapped type of the shape which contains text.

```javascript
isTextWrapped : boolean;
```


### textOrientationType {#textOrientationType--}

Gets and sets the text orientation type of the shape.

```javascript
textOrientationType : TextOrientationType;
```


### textHorizontalAlignment {#textHorizontalAlignment--}

Gets and sets the text horizontal alignment type of the shape.

```javascript
textHorizontalAlignment : TextAlignmentType;
```


### textVerticalAlignment {#textVerticalAlignment--}

Gets and sets the text vertical alignment type of the shape.

```javascript
textVerticalAlignment : TextAlignmentType;
```


### textDirection {#textDirection--}

Gets/Sets the direction of the text flow for this object.

```javascript
textDirection : TextDirectionType;
```


### textBoxOptions {#textBoxOptions--}

Readonly. Gets the text information in the shape

```javascript
textBoxOptions : TextBoxOptions;
```


### controlData {#controlData--}

Readonly. Gets the data of control.

```javascript
controlData : Uint8Array;
```


### activeXControl {#activeXControl--}

Readonly. Gets the ActiveX control.

```javascript
activeXControl : ActiveXControl;
```


### paths {#paths--}

Readonly. Gets the paths of a custom geometric shape.

```javascript
paths : ShapePathCollection;
```


### geometry {#geometry--}

Readonly. Gets the geometry

```javascript
geometry : Geometry;
```


### isDecorative {#isDecorative--}

Indicates whether the object is decorative.

```javascript
isDecorative : boolean;
```


### toFrontOrBack(number) {#toFrontOrBack-number-}

Brings the shape to the front or sends the shape to back.

```javascript
toFrontOrBack(orders: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| orders | number | If it's less than zero, sets the shape to back.         /// If it's greater than zero, brings the shape to front. |

### getLockedProperty(ShapeLockType) {#getLockedProperty-shapelocktype-}

Gets the value of locked property.

```javascript
getLockedProperty(type: ShapeLockType) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [ShapeLockType](../shapelocktype/) | The type of the shape locked property. |

**Returns**

Returns  the value of locked property.

### setLockedProperty(ShapeLockType, boolean) {#setLockedProperty-shapelocktype-boolean-}

Set the locked property.

```javascript
setLockedProperty(type: ShapeLockType, value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [ShapeLockType](../shapelocktype/) | The locked type. |
| value | boolean | The value of the property. |

### addHyperlink(string) {#addHyperlink-string-}

Adds a hyperlink to the shape.

```javascript
addHyperlink(address: string) : Hyperlink;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| address | string | Address of the hyperlink. |

**Returns**

Return the new hyperlink object.

### removeHyperlink() {#removeHyperlink--}

Removes the hyperlink of the shape.

```javascript
removeHyperlink() : void;
```


### moveToRange(number, number, number, number) {#moveToRange-number-number-number-number-}

Moves the shape to a specified range.

```javascript
moveToRange(topRow: number, leftColumn: number, bottomRow: number, rightColumn: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | number | Upper left row index. |
| leftColumn | number | Upper left column index. |
| bottomRow | number | Lower right row index |
| rightColumn | number | Lower right column index |

### alignTopRightCorner(number, number) {#alignTopRightCorner-number-number-}

Moves the picture to the top-right corner.

```javascript
alignTopRightCorner(topRow: number, rightColumn: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | number | the row index. |
| rightColumn | number | the column index. |

### getConnectionPoints() {#getConnectionPoints--}

Get the connection points

```javascript
getConnectionPoints() : number[][];
```


**Returns**

[X,Y] pairs of the connection point. Every item is a float[2] array, [0] represents x and [1] represents y.

### toImageAsync(ImageType) {#toImageAsync-imagetype-}

Creates the shape image and saves it to a stream in the specified format.

```javascript
toImageAsync(imageType: ImageType) : Promise<Uint8Array>;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageType | [ImageType](../imagetype/) | The type in which to save the image. |

**Returns**

The result stream

**Remarks**

The following formats are supported: .bmp, .gif, .jpg, .jpeg, .tiff, .emf.

### toImageAsync(string, ImageOrPrintOptions) {#toImageAsync-string-imageorprintoptions-}

Saves the shape to a file.

```javascript
toImageAsync(imageFile: string, options: ImageOrPrintOptions) : Promise<void>;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | string |  |
| options | [ImageOrPrintOptions](../imageorprintoptions/) |  |

**Returns**

[Promise<void>](../promise<void>/)

### toImageAsync(ImageOrPrintOptions) {#toImageAsync-imageorprintoptions-}

Saves the shape to a stream.

```javascript
toImageAsync(options: ImageOrPrintOptions) : Promise<Uint8Array>;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../imageorprintoptions/) |  |

**Returns**

The result stream

### toImage(ImageType) {#toImage-imagetype-}

Creates the shape image and saves it to a stream in the specified format.

```javascript
toImage(imageType: ImageType) : Uint8Array;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageType | [ImageType](../imagetype/) | The type in which to save the image. |

**Returns**

The result stream

**Remarks**

The following formats are supported: .bmp, .gif, .jpg, .jpeg, .tiff, .emf.

### toImage(string, ImageOrPrintOptions) {#toImage-string-imageorprintoptions-}

Saves the shape to a file.

```javascript
toImage(imageFile: string, options: ImageOrPrintOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | string |  |
| options | [ImageOrPrintOptions](../imageorprintoptions/) |  |

### toImage(ImageOrPrintOptions) {#toImage-imageorprintoptions-}

Saves the shape to a stream.

```javascript
toImage(options: ImageOrPrintOptions) : Uint8Array;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [ImageOrPrintOptions](../imageorprintoptions/) |  |

**Returns**

The result stream

### getLinkedCell(boolean, boolean) {#getLinkedCell-boolean-boolean-}

Gets the range linked to the control's value.

```javascript
getLinkedCell(isR1C1: boolean, isLocal: boolean) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns**

The range linked to the control's value.

### setLinkedCell(string, boolean, boolean) {#setLinkedCell-string-boolean-boolean-}

Sets the range linked to the control's value.

```javascript
setLinkedCell(formula: string, isR1C1: boolean, isLocal: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | The range linked to the control's value. |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

### getInputRange(boolean, boolean) {#getInputRange-boolean-boolean-}

Gets the range used to fill the control.

```javascript
getInputRange(isR1C1: boolean, isLocal: boolean) : string;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns**

The range used to fill the control.

### setInputRange(string, boolean, boolean) {#setInputRange-string-boolean-boolean-}

Sets the range used to fill the control.

```javascript
setInputRange(formula: string, isR1C1: boolean, isLocal: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | The range used to fill the control. |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

### updateSelectedValue() {#updateSelectedValue--}

Update the selected value by the value of the linked cell.

```javascript
updateSelectedValue() : void;
```


### calculateTextSize() {#calculateTextSize--}

Recalculate the text area

```javascript
calculateTextSize() : number[];
```


**Returns**

Text's Size in an array(width and height).

### formatCharacters(number, number, Font, StyleFlag) {#formatCharacters-number-number-font-styleflag-}

Formats some characters with the font setting.

```javascript
formatCharacters(startIndex: number, length: number, font: Font, flag: StyleFlag) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | number | The start index. |
| length | number | The length. |
| font | [Font](../font/) | The font setting. |
| flag | [StyleFlag](../styleflag/) | The flag of the font setting. |

### characters(number, number) {#characters-number-number-}

Returns a Characters object that represents a range of characters within the text.

```javascript
characters(startIndex: number, length: number) : FontSetting;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | number | The index of the start of the character. |
| length | number | The number of characters. |

**Returns**

Characters object.

**Remarks**

This method only works on shape with title.

### getRichFormattings() {#getRichFormattings--}

Returns all Characters objects that represents a range of characters within the text .

```javascript
getRichFormattings() : FontSetting[];
```


**Returns**

All Characters objects

### removeActiveXControl() {#removeActiveXControl--}

Remove activeX control.

```javascript
removeActiveXControl() : void;
```


### getActualBox() {#getActualBox--}

Get the actual position and size of the shape (after applying rotation, flip, etc.)

```javascript
getActualBox() : number[];
```


**Returns**

Return the position and size in the order of x, y, w, h

**Remarks**

Note:The interface is not fully functional, especially the location information is not correct.It is recommended not to use this interface until the function is complete.

### fitToTextSize() {#fitToTextSize--}

Recalculate a text area suitable for displaying all text content.

```javascript
fitToTextSize() : void;
```


### getResultOfSmartArt() {#getResultOfSmartArt--}

Converting smart art to grouped shapes.

```javascript
getResultOfSmartArt() : GroupShape;
```


**Returns**

[GroupShape](../groupshape/)

### isSameSetting(VObject) {#isSameSetting-vobject-}

Returns whether the shape is same.

```javascript
isSameSetting(obj: VObject) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | VObject |  |


