---
title: CommentShape
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the shape of the comment.
type: docs
url: /nodejs-cpp/commentshape/
---

## CommentShape class

Represents the shape of the comment.

```javascript
class CommentShape extends Shape;
```


## Constructors

| Name | Description |
| --- | --- |
| [constructor(Shape)](#constructor-shape-)| Constructs from a parent object convertible to this. |

## Methods

| Method | Description |
| --- | --- |
| [getComment()](#getComment--)| Gets the comment object. |
| [getMacroName()](#getMacroName--)| Gets and sets the name of macro. |
| [setMacroName(string)](#setMacroName-string-)| Gets and sets the name of macro. |
| [isEquation()](#isEquation--)| Indicates whether the shape only contains an equation. |
| [isSmartArt()](#isSmartArt--)| Indicates whether the shape is a smart art. |
| [getZOrderPosition()](#getZOrderPosition--)| Returns the position of a shape in the z-order. |
| [setZOrderPosition(number)](#setZOrderPosition-number-)| Returns the position of a shape in the z-order. |
| [getName()](#getName--)| Gets and sets the name of the shape. |
| [setName(string)](#setName-string-)| Gets and sets the name of the shape. |
| [getAlternativeText()](#getAlternativeText--)| Returns or sets the descriptive (alternative) text string of the [Shape](/nodejs-cpp/shape/) object. |
| [setAlternativeText(string)](#setAlternativeText-string-)| Returns or sets the descriptive (alternative) text string of the [Shape](/nodejs-cpp/shape/) object. |
| [getTitle()](#getTitle--)| Specifies the title (caption) of the current shape object. |
| [setTitle(string)](#setTitle-string-)| Specifies the title (caption) of the current shape object. |
| [getLine()](#getLine--)| Gets line style |
| [getFill()](#getFill--)| Returns a [FillFormat](/nodejs-cpp/fillformat/) object that contains fill formatting properties for the specified shape. |
| [getShadowEffect()](#getShadowEffect--)| Represents a [Drawing.ShadowEffect](/nodejs-cpp/drawing.shadoweffect/) object that specifies shadow effect for the chart element or shape. |
| [getReflection()](#getReflection--)| Represents a [ReflectionEffect](/nodejs-cpp/reflectioneffect/) object that specifies reflection effect for the chart element or shape. |
| [getGlow()](#getGlow--)| Represents a [GlowEffect](/nodejs-cpp/gloweffect/) object that specifies glow effect for the chart element or shape. |
| [getSoftEdges()](#getSoftEdges--)| Gets and sets the radius of blur to apply to the edges, in unit of points. |
| [setSoftEdges(number)](#setSoftEdges-number-)| Gets and sets the radius of blur to apply to the edges, in unit of points. |
| [getThreeDFormat()](#getThreeDFormat--)| Gets and sets 3d format of the shape. |
| [getFormatPicture()](#getFormatPicture--)| Gets and sets the options of the picture format. |
| [isHidden()](#isHidden--)| Indicates whether the object is visible. |
| [setIsHidden(boolean)](#setIsHidden-boolean-)| Indicates whether the object is visible. |
| [isLockAspectRatio()](#isLockAspectRatio--)| True means that aspect ratio of the shape is locked. |
| [setIsLockAspectRatio(boolean)](#setIsLockAspectRatio-boolean-)| True means that aspect ratio of the shape is locked. |
| [isAspectRatioLocked()](#isAspectRatioLocked--)| True means that aspect ratio of the shape is locked. |
| [setIsAspectRatioLocked(boolean)](#setIsAspectRatioLocked-boolean-)| True means that aspect ratio of the shape is locked. |
| [getRotationAngle()](#getRotationAngle--)| Gets and sets the rotation of the shape. |
| [setRotationAngle(number)](#setRotationAngle-number-)| Gets and sets the rotation of the shape. |
| [getHyperlink()](#getHyperlink--)| Gets the hyperlink of the shape. |
| [getId()](#getId--)| Gets the identifier of this shape. |
| [getSpid()](#getSpid--)| Specifies an optional string identifier that an application can use to identify the particular shape. |
| [getSpt()](#getSpt--)| Specifies an optional number that an application can use to associate the particular shape with a defined shape type. |
| [getWorksheet()](#getWorksheet--)| Gets the [Worksheet](/nodejs-cpp/worksheet/) object which contains this shape. |
| [isGroup()](#isGroup--)| Indicates whether this shape is a group shape. |
| [isInGroup()](#isInGroup--)| Indicates whether the shape is grouped. |
| [isWordArt()](#isWordArt--)| Indicates whether this shape is a word art. |
| [getTextEffect()](#getTextEffect--)| Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape. Applies to Shape objects that represent WordArt. |
| [isLocked()](#isLocked--)| True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected. |
| [setIsLocked(boolean)](#setIsLocked-boolean-)| True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected. |
| [isPrintable()](#isPrintable--)| Indicates whether the object is printable. If False, this shape will not be printed when printing. |
| [setIsPrintable(boolean)](#setIsPrintable-boolean-)| Indicates whether the object is printable. If False, this shape will not be printed when printing. |
| [getMsoDrawingType()](#getMsoDrawingType--)| Gets drawing type. |
| [getAutoShapeType()](#getAutoShapeType--)| Gets and sets the auto shape type. |
| [setAutoShapeType(AutoShapeType)](#setAutoShapeType-autoshapetype-)| Gets and sets the auto shape type. |
| [getAnchorType()](#getAnchorType--)| Gets and set the type of the shape anchor placeholder. |
| [setAnchorType(ShapeAnchorType)](#setAnchorType-shapeanchortype-)| Gets and set the type of the shape anchor placeholder. |
| [getPlacement()](#getPlacement--)| Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. |
| [setPlacement(PlacementType)](#setPlacement-placementtype-)| Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. |
| [getUpperLeftRow()](#getUpperLeftRow--)| Represents the top row index. |
| [setUpperLeftRow(number)](#setUpperLeftRow-number-)| Represents the top row index. |
| [getUpperDeltaY()](#getUpperDeltaY--)| Gets or sets the shape's vertical offset from its upper left corner row. |
| [setUpperDeltaY(number)](#setUpperDeltaY-number-)| Gets or sets the shape's vertical offset from its upper left corner row. |
| [getUpperLeftColumn()](#getUpperLeftColumn--)| Represents upper left corner column index. |
| [setUpperLeftColumn(number)](#setUpperLeftColumn-number-)| Represents upper left corner column index. |
| [getUpperDeltaX()](#getUpperDeltaX--)| Gets or sets the shape's horizontal offset from its upper left corner column. |
| [setUpperDeltaX(number)](#setUpperDeltaX-number-)| Gets or sets the shape's horizontal offset from its upper left corner column. |
| [getLowerRightRow()](#getLowerRightRow--)| Represents lower right corner row index. |
| [setLowerRightRow(number)](#setLowerRightRow-number-)| Represents lower right corner row index. |
| [getLowerDeltaY()](#getLowerDeltaY--)| Gets or sets the shape's vertical offset from its lower right corner row. |
| [setLowerDeltaY(number)](#setLowerDeltaY-number-)| Gets or sets the shape's vertical offset from its lower right corner row. |
| [getLowerRightColumn()](#getLowerRightColumn--)| Represents lower right corner column index. |
| [setLowerRightColumn(number)](#setLowerRightColumn-number-)| Represents lower right corner column index. |
| [getLowerDeltaX()](#getLowerDeltaX--)| Gets or sets the shape's horizontal  offset from its lower right corner column. |
| [setLowerDeltaX(number)](#setLowerDeltaX-number-)| Gets or sets the shape's horizontal  offset from its lower right corner column. |
| [getRight()](#getRight--)| Represents the width of the shape's horizontal  offset from its lower right corner column, in unit of pixels. |
| [setRight(number)](#setRight-number-)| Represents the width of the shape's horizontal  offset from its lower right corner column, in unit of pixels. |
| [getBottom()](#getBottom--)| Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels. |
| [setBottom(number)](#setBottom-number-)| Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels. |
| [getWidth()](#getWidth--)| Represents the width of shape, in unit of pixels. |
| [setWidth(number)](#setWidth-number-)| Represents the width of shape, in unit of pixels. |
| [getWidthInch()](#getWidthInch--)| Represents the width of the shape, in unit of inch. |
| [setWidthInch(number)](#setWidthInch-number-)| Represents the width of the shape, in unit of inch. |
| [getWidthPt()](#getWidthPt--)| Represents the width of the shape, in unit of point. |
| [setWidthPt(number)](#setWidthPt-number-)| Represents the width of the shape, in unit of point. |
| [getWidthCM()](#getWidthCM--)| Represents the width of the shape, in unit of centimeters. |
| [setWidthCM(number)](#setWidthCM-number-)| Represents the width of the shape, in unit of centimeters. |
| [getHeight()](#getHeight--)| Represents the height of shape, in unit of pixel. |
| [setHeight(number)](#setHeight-number-)| Represents the height of shape, in unit of pixel. |
| [getHeightInch()](#getHeightInch--)| Represents the height of the shape, in unit of inches. |
| [setHeightInch(number)](#setHeightInch-number-)| Represents the height of the shape, in unit of inches. |
| [getHeightPt()](#getHeightPt--)| Represents the height of the shape, in unit of points. |
| [setHeightPt(number)](#setHeightPt-number-)| Represents the height of the shape, in unit of points. |
| [getHeightCM()](#getHeightCM--)| Represents the height of the shape, in unit of centimeters. |
| [setHeightCM(number)](#setHeightCM-number-)| Represents the height of the shape, in unit of centimeters. |
| [getLeft()](#getLeft--)| Represents the horizontal offset of shape from its left column, in unit of pixels. |
| [setLeft(number)](#setLeft-number-)| Represents the horizontal offset of shape from its left column, in unit of pixels. |
| [getLeftInch()](#getLeftInch--)| Represents the horizontal offset of shape from its left column, in unit of inches. |
| [setLeftInch(number)](#setLeftInch-number-)| Represents the horizontal offset of shape from its left column, in unit of inches. |
| [getLeftCM()](#getLeftCM--)| Represents the horizontal offset of shape from its left column, in unit of centimeters. |
| [setLeftCM(number)](#setLeftCM-number-)| Represents the horizontal offset of shape from its left column, in unit of centimeters. |
| [getTop()](#getTop--)| Represents the vertical offset of shape from its top row, in unit of pixels. |
| [setTop(number)](#setTop-number-)| Represents the vertical offset of shape from its top row, in unit of pixels. |
| [getTopInch()](#getTopInch--)| Represents the vertical offset of shape from its top row, in unit of inches. |
| [setTopInch(number)](#setTopInch-number-)| Represents the vertical offset of shape from its top row, in unit of inches. |
| [getTopCM()](#getTopCM--)| Represents the vertical offset of shape from its top row, in unit of centimeters. |
| [setTopCM(number)](#setTopCM-number-)| Represents the vertical offset of shape from its top row, in unit of centimeters. |
| [getTopToCorner()](#getTopToCorner--)| Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels. |
| [setTopToCorner(number)](#setTopToCorner-number-)| Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels. |
| [getLeftToCorner()](#getLeftToCorner--)| Gets and sets the horizonal offset of shape from worksheet left border. |
| [setLeftToCorner(number)](#setLeftToCorner-number-)| Gets and sets the horizonal offset of shape from worksheet left border. |
| [getX()](#getX--)| Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels. |
| [setX(number)](#setX-number-)| Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels. |
| [getY()](#getY--)| Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels. |
| [setY(number)](#setY-number-)| Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels. |
| [getWidthScale()](#getWidthScale--)| Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100; |
| [setWidthScale(number)](#setWidthScale-number-)| Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100; |
| [getHeightScale()](#getHeightScale--)| Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100; |
| [setHeightScale(number)](#setHeightScale-number-)| Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100; |
| [getTopInShape()](#getTopInShape--)| Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. |
| [setTopInShape(number)](#setTopInShape-number-)| Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. |
| [getLeftInShape()](#getLeftInShape--)| Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. |
| [setLeftInShape(number)](#setLeftInShape-number-)| Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. |
| [getWidthInShape()](#getWidthInShape--)| Represents the width of the shape, in unit of 1/4000 of the parent shape. |
| [setWidthInShape(number)](#setWidthInShape-number-)| Represents the width of the shape, in unit of 1/4000 of the parent shape. |
| [getHeightInShape()](#getHeightInShape--)| Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. |
| [setHeightInShape(number)](#setHeightInShape-number-)| Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. |
| [getGroup()](#getGroup--)| Gets the group shape which contains this shape. |
| [getType()](#getType--)| Gets the auto shape type. |
| [getHasLine()](#getHasLine--)| Gets and sets the line border of the shape is visible. |
| [setHasLine(boolean)](#setHasLine-boolean-)| Gets and sets the line border of the shape is visible. |
| [isFilled()](#isFilled--)| Indicates whether the fill format is visible. |
| [setIsFilled(boolean)](#setIsFilled-boolean-)| Indicates whether the fill format is visible. |
| [isFlippedHorizontally()](#isFlippedHorizontally--)| Gets and sets whether shape is horizontally flipped . |
| [setIsFlippedHorizontally(boolean)](#setIsFlippedHorizontally-boolean-)| Gets and sets whether shape is horizontally flipped . |
| [isFlippedVertically()](#isFlippedVertically--)| Gets and sets whether shape is vertically flipped . |
| [setIsFlippedVertically(boolean)](#setIsFlippedVertically-boolean-)| Gets and sets whether shape is vertically flipped . |
| [getActualLowerRightRow()](#getActualLowerRightRow--)| Get the actual bottom row. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--)| Indicates whether shape is relative to original picture size. |
| [setRelativeToOriginalPictureSize(boolean)](#setRelativeToOriginalPictureSize-boolean-)| Indicates whether shape is relative to original picture size. |
| [getTextShapeType()](#getTextShapeType--)| Gets and sets the preset text shape type. |
| [setTextShapeType(AutoShapeType)](#setTextShapeType-autoshapetype-)| Gets and sets the preset text shape type. |
| [getTextBody()](#getTextBody--)| Gets and sets the setting of the shape's text. |
| [getFont()](#getFont--)| Represents the font of shape. |
| [setFont(Font)](#setFont-font-)| Represents the font of shape. |
| [getTextOptions()](#getTextOptions--)| Represents the text options of the shape. |
| [setTextOptions(TextOptions)](#setTextOptions-textoptions-)| Represents the text options of the shape. |
| [getText()](#getText--)| Gets and sets the text of this shape. |
| [setText(string)](#setText-string-)| Gets and sets the text of this shape. |
| [isRichText()](#isRichText--)| Whether or not the text is rich text. |
| [getHtmlText()](#getHtmlText--)| Gets and sets the html string which contains data and some formats in this textbox. |
| [setHtmlText(string)](#setHtmlText-string-)| Gets and sets the html string which contains data and some formats in this textbox. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--)| Gets and sets the text vertical overflow type of the shape which contains text. |
| [setTextVerticalOverflow(TextOverflowType)](#setTextVerticalOverflow-textoverflowtype-)| Gets and sets the text vertical overflow type of the shape which contains text. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--)| Gets and sets the text horizontal overflow type of the shape which contains text. |
| [setTextHorizontalOverflow(TextOverflowType)](#setTextHorizontalOverflow-textoverflowtype-)| Gets and sets the text horizontal overflow type of the shape which contains text. |
| [isTextWrapped()](#isTextWrapped--)| Gets and sets the text wrapped type of the shape which contains text. |
| [setIsTextWrapped(boolean)](#setIsTextWrapped-boolean-)| Gets and sets the text wrapped type of the shape which contains text. |
| [getTextOrientationType()](#getTextOrientationType--)| Gets and sets the text orientation type of the shape. |
| [setTextOrientationType(TextOrientationType)](#setTextOrientationType-textorientationtype-)| Gets and sets the text orientation type of the shape. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--)| Gets and sets the text horizontal alignment type of the shape. |
| [setTextHorizontalAlignment(TextAlignmentType)](#setTextHorizontalAlignment-textalignmenttype-)| Gets and sets the text horizontal alignment type of the shape. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--)| Gets and sets the text vertical alignment type of the shape. |
| [setTextVerticalAlignment(TextAlignmentType)](#setTextVerticalAlignment-textalignmenttype-)| Gets and sets the text vertical alignment type of the shape. |
| [getTextDirection()](#getTextDirection--)| Gets/Sets the direction of the text flow for this object. |
| [setTextDirection(TextDirectionType)](#setTextDirection-textdirectiontype-)| Gets/Sets the direction of the text flow for this object. |
| [getControlData()](#getControlData--)| Gets the data of control. |
| [getActiveXControl()](#getActiveXControl--)| Gets the ActiveX control. |
| [getPaths()](#getPaths--)| Gets the paths of a custom geometric shape. |
| [getGeometry()](#getGeometry--)| Gets the geometry |
| [isDecorative()](#isDecorative--)| Indicates whether the object is decorative. |
| [setIsDecorative(boolean)](#setIsDecorative-boolean-)| Indicates whether the object is decorative. |
| [getResultOfSmartArt()](#getResultOfSmartArt--)| Converting smart art to grouped shapes. |
| [toFrontOrBack(number)](#toFrontOrBack-number-)| Brings the shape to the front or sends the shape to back. |
| [getLockedProperty(ShapeLockType)](#getLockedProperty-shapelocktype-)| Gets the value of locked property. |
| [setLockedProperty(ShapeLockType, boolean)](#setLockedProperty-shapelocktype-boolean-)| Set the locked property. |
| [addHyperlink(string)](#addHyperlink-string-)| Adds a hyperlink to the shape. |
| [removeHyperlink()](#removeHyperlink--)| Removes the hyperlink of the shape. |
| [moveToRange(number, number, number, number)](#moveToRange-number-number-number-number-)| Moves the shape to a specified range. |
| [alignTopRightCorner(number, number)](#alignTopRightCorner-number-number-)| Moves the picture to the top-right corner. |
| [toImage(Uint8Array, ImageType)](#toImage-uint8array-imagetype-)| Creates the shape image and saves it to a stream in the specified format. |
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


### constructor(Shape) {#constructor-shape-}

Constructs from a parent object convertible to this.

```javascript
constructor(obj: Shape);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | Shape | The parent object. |

### getComment() {#getComment--}

Gets the comment object.

```javascript
getComment() : Comment;
```


**Returns**

[Comment](/nodejs-cpp/comment/)

### getMacroName() {#getMacroName--}

Gets and sets the name of macro.

```javascript
getMacroName() : string;
```


### setMacroName(string) {#setMacroName-string-}

Gets and sets the name of macro.

```javascript
setMacroName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isEquation() {#isEquation--}

Indicates whether the shape only contains an equation.

```javascript
isEquation() : boolean;
```


### isSmartArt() {#isSmartArt--}

Indicates whether the shape is a smart art.

```javascript
isSmartArt() : boolean;
```


**Remarks**

Only for ooxml file.

### getZOrderPosition() {#getZOrderPosition--}

Returns the position of a shape in the z-order.

```javascript
getZOrderPosition() : number;
```


### setZOrderPosition(number) {#setZOrderPosition-number-}

Returns the position of a shape in the z-order.

```javascript
setZOrderPosition(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getName() {#getName--}

Gets and sets the name of the shape.

```javascript
getName() : string;
```


### setName(string) {#setName-string-}

Gets and sets the name of the shape.

```javascript
setName(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getAlternativeText() {#getAlternativeText--}

Returns or sets the descriptive (alternative) text string of the [Shape](/nodejs-cpp/shape/) object.

```javascript
getAlternativeText() : string;
```


### setAlternativeText(string) {#setAlternativeText-string-}

Returns or sets the descriptive (alternative) text string of the [Shape](/nodejs-cpp/shape/) object.

```javascript
setAlternativeText(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getTitle() {#getTitle--}

Specifies the title (caption) of the current shape object.

```javascript
getTitle() : string;
```


### setTitle(string) {#setTitle-string-}

Specifies the title (caption) of the current shape object.

```javascript
setTitle(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getLine() {#getLine--}

Gets line style

```javascript
getLine() : LineFormat;
```


**Returns**

[LineFormat](/nodejs-cpp/lineformat/)

### getFill() {#getFill--}

Returns a [FillFormat](/nodejs-cpp/fillformat/) object that contains fill formatting properties for the specified shape.

```javascript
getFill() : FillFormat;
```


**Returns**

[FillFormat](/nodejs-cpp/fillformat/)

### getShadowEffect() {#getShadowEffect--}

Represents a [Drawing.ShadowEffect](/nodejs-cpp/drawing.shadoweffect/) object that specifies shadow effect for the chart element or shape.

```javascript
getShadowEffect() : ShadowEffect;
```


**Returns**

[ShadowEffect](/nodejs-cpp/shadoweffect/)

### getReflection() {#getReflection--}

Represents a [ReflectionEffect](/nodejs-cpp/reflectioneffect/) object that specifies reflection effect for the chart element or shape.

```javascript
getReflection() : ReflectionEffect;
```


**Returns**

[ReflectionEffect](/nodejs-cpp/reflectioneffect/)

### getGlow() {#getGlow--}

Represents a [GlowEffect](/nodejs-cpp/gloweffect/) object that specifies glow effect for the chart element or shape.

```javascript
getGlow() : GlowEffect;
```


**Returns**

[GlowEffect](/nodejs-cpp/gloweffect/)

### getSoftEdges() {#getSoftEdges--}

Gets and sets the radius of blur to apply to the edges, in unit of points.

```javascript
getSoftEdges() : number;
```


### setSoftEdges(number) {#setSoftEdges-number-}

Gets and sets the radius of blur to apply to the edges, in unit of points.

```javascript
setSoftEdges(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getThreeDFormat() {#getThreeDFormat--}

Gets and sets 3d format of the shape.

```javascript
getThreeDFormat() : ThreeDFormat;
```


**Returns**

[ThreeDFormat](/nodejs-cpp/threedformat/)

### getFormatPicture() {#getFormatPicture--}

Gets and sets the options of the picture format.

```javascript
getFormatPicture() : MsoFormatPicture;
```


**Returns**

[MsoFormatPicture](/nodejs-cpp/msoformatpicture/)

### isHidden() {#isHidden--}

Indicates whether the object is visible.

```javascript
isHidden() : boolean;
```


### setIsHidden(boolean) {#setIsHidden-boolean-}

Indicates whether the object is visible.

```javascript
setIsHidden(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isLockAspectRatio() {#isLockAspectRatio--}

True means that aspect ratio of the shape is locked.

```javascript
isLockAspectRatio() : boolean;
```


**Remarks**

Only for pictures and Ole Objects. NOTE: This member is now obsolete. Instead, please use Shape.IsAspectRatioLocked property. This property will be removed 12 months later since July 2024. Aspose apologizes for any inconvenience you may have experienced.

### setIsLockAspectRatio(boolean) {#setIsLockAspectRatio-boolean-}

True means that aspect ratio of the shape is locked.

```javascript
setIsLockAspectRatio(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only for pictures and Ole Objects. NOTE: This member is now obsolete. Instead, please use Shape.IsAspectRatioLocked property. This property will be removed 12 months later since July 2024. Aspose apologizes for any inconvenience you may have experienced.

### isAspectRatioLocked() {#isAspectRatioLocked--}

True means that aspect ratio of the shape is locked.

```javascript
isAspectRatioLocked() : boolean;
```


**Remarks**

Only for pictures and Ole Objects.

### setIsAspectRatioLocked(boolean) {#setIsAspectRatioLocked-boolean-}

True means that aspect ratio of the shape is locked.

```javascript
setIsAspectRatioLocked(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

**Remarks**

Only for pictures and Ole Objects.

### getRotationAngle() {#getRotationAngle--}

Gets and sets the rotation of the shape.

```javascript
getRotationAngle() : number;
```


### setRotationAngle(number) {#setRotationAngle-number-}

Gets and sets the rotation of the shape.

```javascript
setRotationAngle(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHyperlink() {#getHyperlink--}

Gets the hyperlink of the shape.

```javascript
getHyperlink() : Hyperlink;
```


**Returns**

[Hyperlink](/nodejs-cpp/hyperlink/)

### getId() {#getId--}

Gets the identifier of this shape.

```javascript
getId() : number;
```


### getSpid() {#getSpid--}

Specifies an optional string identifier that an application can use to identify the particular shape.

```javascript
getSpid() : string;
```


### getSpt() {#getSpt--}

Specifies an optional number that an application can use to associate the particular shape with a defined shape type.

```javascript
getSpt() : number;
```


### getWorksheet() {#getWorksheet--}

Gets the [Worksheet](/nodejs-cpp/worksheet/) object which contains this shape.

```javascript
getWorksheet() : Worksheet;
```


**Returns**

[Worksheet](/nodejs-cpp/worksheet/)

### isGroup() {#isGroup--}

Indicates whether this shape is a group shape.

```javascript
isGroup() : boolean;
```


### isInGroup() {#isInGroup--}

Indicates whether the shape is grouped.

```javascript
isInGroup() : boolean;
```


### isWordArt() {#isWordArt--}

Indicates whether this shape is a word art.

```javascript
isWordArt() : boolean;
```


**Remarks**

Only for the Legacy Shape of xls file.

### getTextEffect() {#getTextEffect--}

Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape. Applies to Shape objects that represent WordArt.

```javascript
getTextEffect() : TextEffectFormat;
```


**Returns**

[TextEffectFormat](/nodejs-cpp/texteffectformat/)

### isLocked() {#isLocked--}

True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected.

```javascript
isLocked() : boolean;
```


### setIsLocked(boolean) {#setIsLocked-boolean-}

True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected.

```javascript
setIsLocked(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isPrintable() {#isPrintable--}

Indicates whether the object is printable. If False, this shape will not be printed when printing.

```javascript
isPrintable() : boolean;
```


### setIsPrintable(boolean) {#setIsPrintable-boolean-}

Indicates whether the object is printable. If False, this shape will not be printed when printing.

```javascript
setIsPrintable(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getMsoDrawingType() {#getMsoDrawingType--}

Gets drawing type.

```javascript
getMsoDrawingType() : MsoDrawingType;
```


**Returns**

[MsoDrawingType](/nodejs-cpp/msodrawingtype/)

### getAutoShapeType() {#getAutoShapeType--}

Gets and sets the auto shape type.

```javascript
getAutoShapeType() : AutoShapeType;
```


**Returns**

[AutoShapeType](/nodejs-cpp/autoshapetype/)

### setAutoShapeType(AutoShapeType) {#setAutoShapeType-autoshapetype-}

Gets and sets the auto shape type.

```javascript
setAutoShapeType(value: AutoShapeType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AutoShapeType](/nodejs-cpp/autoshapetype/) | The value to set. |

### getAnchorType() {#getAnchorType--}

Gets and set the type of the shape anchor placeholder.

```javascript
getAnchorType() : ShapeAnchorType;
```


**Returns**

[ShapeAnchorType](/nodejs-cpp/shapeanchortype/)

### setAnchorType(ShapeAnchorType) {#setAnchorType-shapeanchortype-}

Gets and set the type of the shape anchor placeholder.

```javascript
setAnchorType(value: ShapeAnchorType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ShapeAnchorType](/nodejs-cpp/shapeanchortype/) | The value to set. |

### getPlacement() {#getPlacement--}

Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.

```javascript
getPlacement() : PlacementType;
```


**Returns**

[PlacementType](/nodejs-cpp/placementtype/)

### setPlacement(PlacementType) {#setPlacement-placementtype-}

Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.

```javascript
setPlacement(value: PlacementType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PlacementType](/nodejs-cpp/placementtype/) | The value to set. |

### getUpperLeftRow() {#getUpperLeftRow--}

Represents the top row index.

```javascript
getUpperLeftRow() : number;
```


**Remarks**

If the shape is in the shape or in the group , UpperLeftRow will be ignored.

### setUpperLeftRow(number) {#setUpperLeftRow-number-}

Represents the top row index.

```javascript
setUpperLeftRow(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

If the shape is in the shape or in the group , UpperLeftRow will be ignored.

### getUpperDeltaY() {#getUpperDeltaY--}

Gets or sets the shape's vertical offset from its upper left corner row.

```javascript
getUpperDeltaY() : number;
```


**Remarks**

The range of value is 0 to 256.

### setUpperDeltaY(number) {#setUpperDeltaY-number-}

Gets or sets the shape's vertical offset from its upper left corner row.

```javascript
setUpperDeltaY(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The range of value is 0 to 256.

### getUpperLeftColumn() {#getUpperLeftColumn--}

Represents upper left corner column index.

```javascript
getUpperLeftColumn() : number;
```


### setUpperLeftColumn(number) {#setUpperLeftColumn-number-}

Represents upper left corner column index.

```javascript
setUpperLeftColumn(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getUpperDeltaX() {#getUpperDeltaX--}

Gets or sets the shape's horizontal offset from its upper left corner column.

```javascript
getUpperDeltaX() : number;
```


**Remarks**

The range of value is 0 to 1024.

### setUpperDeltaX(number) {#setUpperDeltaX-number-}

Gets or sets the shape's horizontal offset from its upper left corner column.

```javascript
setUpperDeltaX(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The range of value is 0 to 1024.

### getLowerRightRow() {#getLowerRightRow--}

Represents lower right corner row index.

```javascript
getLowerRightRow() : number;
```


### setLowerRightRow(number) {#setLowerRightRow-number-}

Represents lower right corner row index.

```javascript
setLowerRightRow(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getLowerDeltaY() {#getLowerDeltaY--}

Gets or sets the shape's vertical offset from its lower right corner row.

```javascript
getLowerDeltaY() : number;
```


**Remarks**

The range of value is 0 to 256.

### setLowerDeltaY(number) {#setLowerDeltaY-number-}

Gets or sets the shape's vertical offset from its lower right corner row.

```javascript
setLowerDeltaY(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The range of value is 0 to 256.

### getLowerRightColumn() {#getLowerRightColumn--}

Represents lower right corner column index.

```javascript
getLowerRightColumn() : number;
```


### setLowerRightColumn(number) {#setLowerRightColumn-number-}

Represents lower right corner column index.

```javascript
setLowerRightColumn(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getLowerDeltaX() {#getLowerDeltaX--}

Gets or sets the shape's horizontal  offset from its lower right corner column.

```javascript
getLowerDeltaX() : number;
```


**Remarks**

The range of value is 0 to 1024.

### setLowerDeltaX(number) {#setLowerDeltaX-number-}

Gets or sets the shape's horizontal  offset from its lower right corner column.

```javascript
setLowerDeltaX(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

The range of value is 0 to 1024.

### getRight() {#getRight--}

Represents the width of the shape's horizontal  offset from its lower right corner column, in unit of pixels.

```javascript
getRight() : number;
```


### setRight(number) {#setRight-number-}

Represents the width of the shape's horizontal  offset from its lower right corner column, in unit of pixels.

```javascript
setRight(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getBottom() {#getBottom--}

Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels.

```javascript
getBottom() : number;
```


### setBottom(number) {#setBottom-number-}

Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels.

```javascript
setBottom(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWidth() {#getWidth--}

Represents the width of shape, in unit of pixels.

```javascript
getWidth() : number;
```


### setWidth(number) {#setWidth-number-}

Represents the width of shape, in unit of pixels.

```javascript
setWidth(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWidthInch() {#getWidthInch--}

Represents the width of the shape, in unit of inch.

```javascript
getWidthInch() : number;
```


### setWidthInch(number) {#setWidthInch-number-}

Represents the width of the shape, in unit of inch.

```javascript
setWidthInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWidthPt() {#getWidthPt--}

Represents the width of the shape, in unit of point.

```javascript
getWidthPt() : number;
```


### setWidthPt(number) {#setWidthPt-number-}

Represents the width of the shape, in unit of point.

```javascript
setWidthPt(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWidthCM() {#getWidthCM--}

Represents the width of the shape, in unit of centimeters.

```javascript
getWidthCM() : number;
```


### setWidthCM(number) {#setWidthCM-number-}

Represents the width of the shape, in unit of centimeters.

```javascript
setWidthCM(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHeight() {#getHeight--}

Represents the height of shape, in unit of pixel.

```javascript
getHeight() : number;
```


### setHeight(number) {#setHeight-number-}

Represents the height of shape, in unit of pixel.

```javascript
setHeight(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHeightInch() {#getHeightInch--}

Represents the height of the shape, in unit of inches.

```javascript
getHeightInch() : number;
```


### setHeightInch(number) {#setHeightInch-number-}

Represents the height of the shape, in unit of inches.

```javascript
setHeightInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHeightPt() {#getHeightPt--}

Represents the height of the shape, in unit of points.

```javascript
getHeightPt() : number;
```


### setHeightPt(number) {#setHeightPt-number-}

Represents the height of the shape, in unit of points.

```javascript
setHeightPt(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHeightCM() {#getHeightCM--}

Represents the height of the shape, in unit of centimeters.

```javascript
getHeightCM() : number;
```


### setHeightCM(number) {#setHeightCM-number-}

Represents the height of the shape, in unit of centimeters.

```javascript
setHeightCM(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getLeft() {#getLeft--}

Represents the horizontal offset of shape from its left column, in unit of pixels.

```javascript
getLeft() : number;
```


### setLeft(number) {#setLeft-number-}

Represents the horizontal offset of shape from its left column, in unit of pixels.

```javascript
setLeft(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getLeftInch() {#getLeftInch--}

Represents the horizontal offset of shape from its left column, in unit of inches.

```javascript
getLeftInch() : number;
```


### setLeftInch(number) {#setLeftInch-number-}

Represents the horizontal offset of shape from its left column, in unit of inches.

```javascript
setLeftInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getLeftCM() {#getLeftCM--}

Represents the horizontal offset of shape from its left column, in unit of centimeters.

```javascript
getLeftCM() : number;
```


### setLeftCM(number) {#setLeftCM-number-}

Represents the horizontal offset of shape from its left column, in unit of centimeters.

```javascript
setLeftCM(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getTop() {#getTop--}

Represents the vertical offset of shape from its top row, in unit of pixels.

```javascript
getTop() : number;
```


**Remarks**

If the shape is in the chart, represents the vertical offset of shape from its top border.

### setTop(number) {#setTop-number-}

Represents the vertical offset of shape from its top row, in unit of pixels.

```javascript
setTop(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

If the shape is in the chart, represents the vertical offset of shape from its top border.

### getTopInch() {#getTopInch--}

Represents the vertical offset of shape from its top row, in unit of inches.

```javascript
getTopInch() : number;
```


### setTopInch(number) {#setTopInch-number-}

Represents the vertical offset of shape from its top row, in unit of inches.

```javascript
setTopInch(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getTopCM() {#getTopCM--}

Represents the vertical offset of shape from its top row, in unit of centimeters.

```javascript
getTopCM() : number;
```


### setTopCM(number) {#setTopCM-number-}

Represents the vertical offset of shape from its top row, in unit of centimeters.

```javascript
setTopCM(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getTopToCorner() {#getTopToCorner--}

Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels.

```javascript
getTopToCorner() : number;
```


### setTopToCorner(number) {#setTopToCorner-number-}

Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels.

```javascript
setTopToCorner(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getLeftToCorner() {#getLeftToCorner--}

Gets and sets the horizonal offset of shape from worksheet left border.

```javascript
getLeftToCorner() : number;
```


### setLeftToCorner(number) {#setLeftToCorner-number-}

Gets and sets the horizonal offset of shape from worksheet left border.

```javascript
setLeftToCorner(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getX() {#getX--}

Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels.

```javascript
getX() : number;
```


### setX(number) {#setX-number-}

Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels.

```javascript
setX(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getY() {#getY--}

Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels.

```javascript
getY() : number;
```


### setY(number) {#setY-number-}

Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels.

```javascript
setY(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getWidthScale() {#getWidthScale--}

Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100;

```javascript
getWidthScale() : number;
```


### setWidthScale(number) {#setWidthScale-number-}

Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100;

```javascript
setWidthScale(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getHeightScale() {#getHeightScale--}

Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100;

```javascript
getHeightScale() : number;
```


### setHeightScale(number) {#setHeightScale-number-}

Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100;

```javascript
setHeightScale(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

### getTopInShape() {#getTopInShape--}

Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.

```javascript
getTopInShape() : number;
```


**Remarks**

Only Applies when this shape in the group or chart.

### setTopInShape(number) {#setTopInShape-number-}

Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.

```javascript
setTopInShape(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

Only Applies when this shape in the group or chart.

### getLeftInShape() {#getLeftInShape--}

Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape.

```javascript
getLeftInShape() : number;
```


**Remarks**

Only Applies when this shape in the group or chart.

### setLeftInShape(number) {#setLeftInShape-number-}

Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape.

```javascript
setLeftInShape(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

Only Applies when this shape in the group or chart.

### getWidthInShape() {#getWidthInShape--}

Represents the width of the shape, in unit of 1/4000 of the parent shape.

```javascript
getWidthInShape() : number;
```


**Remarks**

Only Applies when this shape in the group or chart.

### setWidthInShape(number) {#setWidthInShape-number-}

Represents the width of the shape, in unit of 1/4000 of the parent shape.

```javascript
setWidthInShape(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

Only Applies when this shape in the group or chart.

### getHeightInShape() {#getHeightInShape--}

Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape..

```javascript
getHeightInShape() : number;
```


**Remarks**

Only Applies when this shape in the group or chart.

### setHeightInShape(number) {#setHeightInShape-number-}

Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape..

```javascript
setHeightInShape(value: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |

**Remarks**

Only Applies when this shape in the group or chart.

### getGroup() {#getGroup--}

Gets the group shape which contains this shape.

```javascript
getGroup() : GroupShape;
```


**Returns**

[GroupShape](/nodejs-cpp/groupshape/)

### getType() {#getType--}

Gets the auto shape type.

```javascript
getType() : AutoShapeType;
```


**Returns**

[AutoShapeType](/nodejs-cpp/autoshapetype/)

### getHasLine() {#getHasLine--}

Gets and sets the line border of the shape is visible.

```javascript
getHasLine() : boolean;
```


### setHasLine(boolean) {#setHasLine-boolean-}

Gets and sets the line border of the shape is visible.

```javascript
setHasLine(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isFilled() {#isFilled--}

Indicates whether the fill format is visible.

```javascript
isFilled() : boolean;
```


### setIsFilled(boolean) {#setIsFilled-boolean-}

Indicates whether the fill format is visible.

```javascript
setIsFilled(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isFlippedHorizontally() {#isFlippedHorizontally--}

Gets and sets whether shape is horizontally flipped .

```javascript
isFlippedHorizontally() : boolean;
```


### setIsFlippedHorizontally(boolean) {#setIsFlippedHorizontally-boolean-}

Gets and sets whether shape is horizontally flipped .

```javascript
setIsFlippedHorizontally(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### isFlippedVertically() {#isFlippedVertically--}

Gets and sets whether shape is vertically flipped .

```javascript
isFlippedVertically() : boolean;
```


### setIsFlippedVertically(boolean) {#setIsFlippedVertically-boolean-}

Gets and sets whether shape is vertically flipped .

```javascript
setIsFlippedVertically(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getActualLowerRightRow() {#getActualLowerRightRow--}

Get the actual bottom row.

```javascript
getActualLowerRightRow() : number;
```


### getRelativeToOriginalPictureSize() {#getRelativeToOriginalPictureSize--}

Indicates whether shape is relative to original picture size.

```javascript
getRelativeToOriginalPictureSize() : boolean;
```


### setRelativeToOriginalPictureSize(boolean) {#setRelativeToOriginalPictureSize-boolean-}

Indicates whether shape is relative to original picture size.

```javascript
setRelativeToOriginalPictureSize(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getTextShapeType() {#getTextShapeType--}

Gets and sets the preset text shape type.

```javascript
getTextShapeType() : AutoShapeType;
```


**Returns**

[AutoShapeType](/nodejs-cpp/autoshapetype/)

### setTextShapeType(AutoShapeType) {#setTextShapeType-autoshapetype-}

Gets and sets the preset text shape type.

```javascript
setTextShapeType(value: AutoShapeType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AutoShapeType](/nodejs-cpp/autoshapetype/) | The value to set. |

### getTextBody() {#getTextBody--}

Gets and sets the setting of the shape's text.

```javascript
getTextBody() : FontSettingCollection;
```


**Returns**

[FontSettingCollection](/nodejs-cpp/fontsettingcollection/)

### getFont() {#getFont--}

Represents the font of shape.

```javascript
getFont() : Font;
```


**Returns**

[Font](/nodejs-cpp/font/)

### setFont(Font) {#setFont-font-}

Represents the font of shape.

```javascript
setFont(value: Font) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Font](/nodejs-cpp/font/) | The value to set. |

### getTextOptions() {#getTextOptions--}

Represents the text options of the shape.

```javascript
getTextOptions() : TextOptions;
```


**Returns**

[TextOptions](/nodejs-cpp/textoptions/)

### setTextOptions(TextOptions) {#setTextOptions-textoptions-}

Represents the text options of the shape.

```javascript
setTextOptions(value: TextOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextOptions](/nodejs-cpp/textoptions/) | The value to set. |

### getText() {#getText--}

Gets and sets the text of this shape.

```javascript
getText() : string;
```


### setText(string) {#setText-string-}

Gets and sets the text of this shape.

```javascript
setText(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### isRichText() {#isRichText--}

Whether or not the text is rich text.

```javascript
isRichText() : boolean;
```


### getHtmlText() {#getHtmlText--}

Gets and sets the html string which contains data and some formats in this textbox.

```javascript
getHtmlText() : string;
```


### setHtmlText(string) {#setHtmlText-string-}

Gets and sets the html string which contains data and some formats in this textbox.

```javascript
setHtmlText(value: string) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |

### getTextVerticalOverflow() {#getTextVerticalOverflow--}

Gets and sets the text vertical overflow type of the shape which contains text.

```javascript
getTextVerticalOverflow() : TextOverflowType;
```


**Returns**

[TextOverflowType](/nodejs-cpp/textoverflowtype/)

### setTextVerticalOverflow(TextOverflowType) {#setTextVerticalOverflow-textoverflowtype-}

Gets and sets the text vertical overflow type of the shape which contains text.

```javascript
setTextVerticalOverflow(value: TextOverflowType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextOverflowType](/nodejs-cpp/textoverflowtype/) | The value to set. |

### getTextHorizontalOverflow() {#getTextHorizontalOverflow--}

Gets and sets the text horizontal overflow type of the shape which contains text.

```javascript
getTextHorizontalOverflow() : TextOverflowType;
```


**Returns**

[TextOverflowType](/nodejs-cpp/textoverflowtype/)

### setTextHorizontalOverflow(TextOverflowType) {#setTextHorizontalOverflow-textoverflowtype-}

Gets and sets the text horizontal overflow type of the shape which contains text.

```javascript
setTextHorizontalOverflow(value: TextOverflowType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextOverflowType](/nodejs-cpp/textoverflowtype/) | The value to set. |

### isTextWrapped() {#isTextWrapped--}

Gets and sets the text wrapped type of the shape which contains text.

```javascript
isTextWrapped() : boolean;
```


### setIsTextWrapped(boolean) {#setIsTextWrapped-boolean-}

Gets and sets the text wrapped type of the shape which contains text.

```javascript
setIsTextWrapped(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getTextOrientationType() {#getTextOrientationType--}

Gets and sets the text orientation type of the shape.

```javascript
getTextOrientationType() : TextOrientationType;
```


**Returns**

[TextOrientationType](/nodejs-cpp/textorientationtype/)

### setTextOrientationType(TextOrientationType) {#setTextOrientationType-textorientationtype-}

Gets and sets the text orientation type of the shape.

```javascript
setTextOrientationType(value: TextOrientationType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextOrientationType](/nodejs-cpp/textorientationtype/) | The value to set. |

### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}

Gets and sets the text horizontal alignment type of the shape.

```javascript
getTextHorizontalAlignment() : TextAlignmentType;
```


**Returns**

[TextAlignmentType](/nodejs-cpp/textalignmenttype/)

### setTextHorizontalAlignment(TextAlignmentType) {#setTextHorizontalAlignment-textalignmenttype-}

Gets and sets the text horizontal alignment type of the shape.

```javascript
setTextHorizontalAlignment(value: TextAlignmentType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](/nodejs-cpp/textalignmenttype/) | The value to set. |

### getTextVerticalAlignment() {#getTextVerticalAlignment--}

Gets and sets the text vertical alignment type of the shape.

```javascript
getTextVerticalAlignment() : TextAlignmentType;
```


**Returns**

[TextAlignmentType](/nodejs-cpp/textalignmenttype/)

### setTextVerticalAlignment(TextAlignmentType) {#setTextVerticalAlignment-textalignmenttype-}

Gets and sets the text vertical alignment type of the shape.

```javascript
setTextVerticalAlignment(value: TextAlignmentType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextAlignmentType](/nodejs-cpp/textalignmenttype/) | The value to set. |

### getTextDirection() {#getTextDirection--}

Gets/Sets the direction of the text flow for this object.

```javascript
getTextDirection() : TextDirectionType;
```


**Returns**

[TextDirectionType](/nodejs-cpp/textdirectiontype/)

### setTextDirection(TextDirectionType) {#setTextDirection-textdirectiontype-}

Gets/Sets the direction of the text flow for this object.

```javascript
setTextDirection(value: TextDirectionType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextDirectionType](/nodejs-cpp/textdirectiontype/) | The value to set. |

### getControlData() {#getControlData--}

Gets the data of control.

```javascript
getControlData() : number[];
```


**Returns**

number[]

### getActiveXControl() {#getActiveXControl--}

Gets the ActiveX control.

```javascript
getActiveXControl() : ActiveXControl;
```


**Returns**

[ActiveXControl](/nodejs-cpp/activexcontrol/)

### getPaths() {#getPaths--}

Gets the paths of a custom geometric shape.

```javascript
getPaths() : ShapePathCollection;
```


**Returns**

[ShapePathCollection](/nodejs-cpp/shapepathcollection/)

### getGeometry() {#getGeometry--}

Gets the geometry

```javascript
getGeometry() : Geometry;
```


**Returns**

[Geometry](/nodejs-cpp/geometry/)

### isDecorative() {#isDecorative--}

Indicates whether the object is decorative.

```javascript
isDecorative() : boolean;
```


### setIsDecorative(boolean) {#setIsDecorative-boolean-}

Indicates whether the object is decorative.

```javascript
setIsDecorative(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getResultOfSmartArt() {#getResultOfSmartArt--}

Converting smart art to grouped shapes.

```javascript
getResultOfSmartArt() : GroupShape;
```


**Returns**

[GroupShape](/nodejs-cpp/groupshape/)

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
| type | [ShapeLockType](/nodejs-cpp/shapelocktype/) | The type of the shape locked property. |

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
| type | [ShapeLockType](/nodejs-cpp/shapelocktype/) | The locked type. |
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
moveToRange(upperLeftRow: number, upperLeftColumn: number, lowerRightRow: number, lowerRightColumn: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | number | Upper left row index. |
| upperLeftColumn | number | Upper left column index. |
| lowerRightRow | number | Lower right row index |
| lowerRightColumn | number | Lower right column index |

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

### toImage(Uint8Array, ImageType) {#toImage-uint8array-imagetype-}

Creates the shape image and saves it to a stream in the specified format.

```javascript
toImage(stream: Uint8Array, imageType: ImageType) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | Uint8Array | The output stream. |
| imageType | [ImageType](/nodejs-cpp/imagetype/) | The type in which to save the image. |

**Remarks**

<p>The following formats are supported: .bmp, .gif, .jpg, .jpeg, .tiff, .emf.</p>

### toImage(string, ImageOrPrintOptions) {#toImage-string-imageorprintoptions-}

Saves the shape to a file.

```javascript
toImage(imageFile: string, options: ImageOrPrintOptions) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | string |  |
| options | [ImageOrPrintOptions](/nodejs-cpp/imageorprintoptions/) |  |

### toImage(ImageOrPrintOptions) {#toImage-imageorprintoptions-}

Saves the shape to a stream.

```javascript
toImage(options: ImageOrPrintOptions) : Uint8Array;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| options | [ImageOrPrintOptions](/nodejs-cpp/imageorprintoptions/) |  |

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
| font | [Font](/nodejs-cpp/font/) | The font setting. |
| flag | [StyleFlag](/nodejs-cpp/styleflag/) | The flag of the font setting. |

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


