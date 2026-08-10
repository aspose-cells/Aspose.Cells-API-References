---
title: "ComboBox"
linktitle: "ComboBox"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Represents the control form ComboBox."
type: docs
weight: 700
url: /nodejs/aspose.cells/combobox/
---

## ComboBox class

Represents the control form ComboBox.

## Methods

| Name | Description |
| --- | --- |
| [addHyperlink(address)](#addhyperlink) | Adds a hyperlink to the shape. |
| [alignTopRightCorner(topRow, rightColumn)](#aligntoprightcorner) | Moves the picture to the top-right corner. |
| [calculateTextSize()](#calculatetextsize) | Recalculate the text area |
| [characters(startIndex, length)](#characters) | Returns a Characters object that represents a range of characters within the text. This method only works on shape with  |
| [fitToTextSize()](#fittotextsize) |  |
| [formatCharacters(startIndex, length, font, flag)](#formatcharacters) | Formats some characters with the font setting. |
| [getActualBox()](#getactualbox) | Get the actual position and size of the shape (after applying rotation, flip, etc.) Note:The interface is not fully func |
| [getActualLowerRightRow()](#getactuallowerrightrow) | Get the actual bottom row. |
| [getAlternativeText()](#getalternativetext) | Returns or sets the descriptive (alternative) text string of the Shape object. |
| [getAnchorType()](#getanchortype) | Gets and set the type of the shape anchor placeholder. The value of the property is ShapeAnchorType integer constant. |
| [getAutoShapeType()](#getautoshapetype) | Gets and sets the auto shape type. The value of the property is AutoShapeType integer constant. |
| [getBottom()](#getbottom) | Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels. |
| [getCharacters()](#getcharacters) | Returns all Characters objects that represents a range of characters within the text . NOTE: This method is now obsolete |
| [getConnectionPoints()](#getconnectionpoints) | Get the connection points |
| [getControlData()](#getcontroldata) | Gets the data of control. |
| [getCreateId()](#getcreateid) | Gets and sets create id for this shape. |
| [getDropDownLines()](#getdropdownlines) | Gets or sets the number of list lines displayed in the drop-down portion of a combo box. |
| [getFill()](#getfill) | Returns a FillFormat object that contains fill formatting properties for the specified shape. |
| [getFillFormat()](#getfillformat) | Returns a MsoFillFormat object that contains fill formatting properties for the specified shape. NOTE: This member is no |
| [getFont()](#getfont) | Represents the font of shape. |
| [getFormatPicture()](#getformatpicture) | Gets and sets the options of the picture format. |
| [getGeometry()](#getgeometry) | Gets the geometry |
| [getGlow()](#getglow) | Represents a GlowEffect object that specifies glow effect for the chart element or shape. |
| [getGroup()](#getgroup) | Gets the group shape which contains this shape. |
| [getHeight()](#getheight) | Represents the height of shape, in unit of pixel. |
| [getHeightCM()](#getheightcm) | Represents the height of the shape, in unit of centimeters. |
| [getHeightInShape()](#getheightinshape) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the pare |
| [getHeightInch()](#getheightinch) | Represents the height of the shape, in unit of inches. |
| [getHeightPt()](#getheightpt) | Represents the height of the shape, in unit of points. |
| [getHeightScale()](#getheightscale) | Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the Heigh |
| [getHtmlText()](#gethtmltext) | Gets and sets the html string which contains data and some formats in this textbox. |
| [getHyperlink()](#gethyperlink) | Gets the hyperlink of the shape. |
| [getId()](#getid) | Gets the identifier of this shape. |
| [getInputRange()](#getinputrange) | Gets or sets the worksheet range used to fill the specified combo box. |
| [getInputRange(isR1C1, isLocal)](#getinputrange-1) | Gets the range used to fill the control. |
| [getLeft()](#getleft) | Represents the horizontal offset of shape from its left column, in unit of pixels. |
| [getLeftCM()](#getleftcm) | Represents the horizontal offset of shape from its left column, in unit of centimeters. |
| [getLeftInShape()](#getleftinshape) | Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the pa |
| [getLeftInch()](#getleftinch) | Represents the horizontal offset of shape from its left column, in unit of inches. |
| [getLeftToCorner()](#getlefttocorner) | Gets and sets the horizonal offset of shape from worksheet left border. |
| [getLine()](#getline) | Gets line style |
| [getLineFormat()](#getlineformat) | Returns a MsoLineFormat object that contains line formatting properties for the specified shape. NOTE: This member is no |
| [getLinkedCell()](#getlinkedcell) | Gets or sets the worksheet range linked to the control's value. |
| [getLinkedCell(isR1C1, isLocal)](#getlinkedcell-1) | Gets the range linked to the control's value. |
| [getLockedProperty(type)](#getlockedproperty) | Gets the value of locked property. |
| [getLowerDeltaX()](#getlowerdeltax) | Gets or sets the shape's horizontal offset from its lower right corner column. The range of value is 0 to 1024. |
| [getLowerDeltaY()](#getlowerdeltay) | Gets or sets the shape's vertical offset from its lower right corner row. The range of value is 0 to 256. |
| [getLowerRightColumn()](#getlowerrightcolumn) | Represents lower right corner column index. |
| [getLowerRightRow()](#getlowerrightrow) | Represents lower right corner row index. |
| [getMacroName()](#getmacroname) | Gets and sets the name of macro. |
| [getMsoDrawingType()](#getmsodrawingtype) | Gets drawing type. The value of the property is MsoDrawingType integer constant. |
| [getName()](#getname) | Gets and sets the name of the shape. |
| [getPaths()](#getpaths) | Gets the paths of a custom geometric shape. |
| [getPlacement()](#getplacement) | Represents the way the drawing object is attached to the cells below it. The property controls the placement of an objec |
| [getReflection()](#getreflection) | Represents a ReflectionEffect object that specifies reflection effect for the chart element or shape. |
| [getRelativeToOriginalPictureSize()](#getrelativetooriginalpicturesize) | Indicates whether shape is relative to original picture size. |
| [getResultOfSmartArt()](#getresultofsmartart) | Converting smart art to grouped shapes. |
| [getRichFormattings()](#getrichformattings) | Returns all Characters objects that represents a range of characters within the text . |
| [getRight()](#getright) | Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels. |
| [getRotationAngle()](#getrotationangle) | Gets and sets the rotation of the shape. |
| [getSelectedCell()](#getselectedcell) | Gets the selected cell in the input range of the combo box. |
| [getSelectedIndex()](#getselectedindex) | Gets or sets the index number of the currently selected item in a list box or combo box. Zero-based. -1 presents no item |
| [getSelectedValue()](#getselectedvalue) | Gets the selected value of the combox box. |
| [getShadow()](#getshadow) | Indicates whether the combobox has 3-D shading. |
| [getShadowEffect()](#getshadoweffect) | Represents a ShadowEffect object that specifies shadow effect for the chart element or shape. |
| [getSoftEdges()](#getsoftedges) | Gets and sets the radius of blur to apply to the edges, in unit of points. |
| [getSpid()](#getspid) | Specifies an optional string identifier that an application can use to identify the particular shape. |
| [getSpt()](#getspt) | Specifies an optional number that an application can use to associate the particular shape with a defined shape type. |
| [getText()](#gettext) | Gets and sets the text of this shape. |
| [getTextBody()](#gettextbody) | Gets and sets the setting of the shape's text. |
| [getTextBoxOptions()](#gettextboxoptions) |  |
| [getTextDirection()](#gettextdirection) | Gets/Sets the direction of the text flow for this object. The value of the property is TextDirectionType integer constan |
| [getTextEffect()](#gettexteffect) | Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape. Applies to Sh |
| [getTextHorizontalAlignment()](#gettexthorizontalalignment) | Gets and sets the text horizontal alignment type of the shape. The value of the property is TextAlignmentType integer co |
| [getTextHorizontalOverflow()](#gettexthorizontaloverflow) | Gets and sets the text horizontal overflow type of the shape which contains text. The value of the property is TextOverf |
| [getTextOptions()](#gettextoptions) | Represents the text options of the shape. |
| [getTextOrientationType()](#gettextorientationtype) | Gets and sets the text orientation type of the shape. The value of the property is TextOrientationType integer constant. |
| [getTextShapeType()](#gettextshapetype) | Gets and sets the preset text shape type. The value of the property is AutoShapeType integer constant. |
| [getTextVerticalAlignment()](#gettextverticalalignment) | Gets and sets the text vertical alignment type of the shape. The value of the property is TextAlignmentType integer cons |
| [getTextVerticalOverflow()](#gettextverticaloverflow) | Gets and sets the text vertical overflow type of the shape which contains text. The value of the property is TextOverflo |
| [getThreeDFormat()](#getthreedformat) | Gets and sets 3d format of the shape. |
| [getTitle()](#gettitle) | Specifies the title (caption) of the current shape object. |
| [getTop()](#gettop) | Represents the vertical offset of shape from its top row, in unit of pixels. If the shape is in the chart, represents th |
| [getTopCM()](#gettopcm) | Represents the vertical offset of shape from its top row, in unit of centimeters. |
| [getTopInShape()](#gettopinshape) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the pare |
| [getTopInch()](#gettopinch) | Represents the vertical offset of shape from its top row, in unit of inches. |
| [getTopToCorner()](#gettoptocorner) | Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels. |
| [getType()](#gettype) | Gets the auto shape type. The value of the property is AutoShapeType integer constant. |
| [getUpperDeltaX()](#getupperdeltax) | Gets or sets the shape's horizontal offset from its upper left corner column. The range of value is 0 to 1024. |
| [getUpperDeltaY()](#getupperdeltay) | Gets or sets the shape's vertical offset from its upper left corner row. The range of value is 0 to 256. |
| [getUpperLeftColumn()](#getupperleftcolumn) | Represents upper left corner column index. |
| [getUpperLeftRow()](#getupperleftrow) | Represents the top row index. If the shape is in the shape or in the group , UpperLeftRow will be ignored. |
| [getWidth()](#getwidth) | Represents the width of shape, in unit of pixels. |
| [getWidthCM()](#getwidthcm) | Represents the width of the shape, in unit of centimeters. |
| [getWidthInShape()](#getwidthinshape) | Represents the width of the shape, in unit of 1/4000 of the parent shape. Only Applies when this shape in the group or c |
| [getWidthInch()](#getwidthinch) | Represents the width of the shape, in unit of inch. |
| [getWidthPt()](#getwidthpt) | Represents the width of the shape, in unit of point. |
| [getWidthScale()](#getwidthscale) | Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthS |
| [getWorksheet()](#getworksheet) | Gets the Worksheet object which contains this shape. |
| [getX()](#getx) | Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels. |
| [getY()](#gety) | Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels. |
| [getZOrderPosition()](#getzorderposition) | Returns the position of a shape in the z-order. |
| [hasLine()](#hasline) | Gets and sets the line border of the shape is visible. |
| [isAspectRatioLocked()](#isaspectratiolocked) | True means that aspect ratio of the shape is locked. Only for pictures and Ole Objects. |
| [isDecorative()](#isdecorative) |  |
| [isEquation()](#isequation) | Indicates whether the shape only contains an equation. |
| [isFilled()](#isfilled) | Indicates whether the fill format is visible. |
| [isFlippedHorizontally()](#isflippedhorizontally) | Gets and sets whether shape is horizontally flipped . |
| [isFlippedVertically()](#isflippedvertically) | Gets and sets whether shape is vertically flipped . |
| [isGroup()](#isgroup) | Indicates whether this shape is a group shape. |
| [isHidden()](#ishidden) | Indicates whether the object is visible. |
| [isInGroup()](#isingroup) | Indicates whether the shape is grouped. |
| [isLockAspectRatio()](#islockaspectratio) | True means that aspect ratio of the shape is locked. Only for pictures and Ole Objects. NOTE: This member is now obsolet |
| [isLocked()](#islocked) | True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the wo |
| [isPrintable()](#isprintable) | Indicates whether the object is printable. If False, this shape will not be printed when printing. |
| [isRichText()](#isrichtext) | Whether or not the text is rich text. |
| [isSameSetting(obj)](#issamesetting) | Returns whether the shape is same. |
| [isSmartArt()](#issmartart) | Indicates whether the shape is a smart art. Only for ooxml file. |
| [isTextWrapped()](#istextwrapped) | Gets and sets the text wrapped type of the shape which contains text. |
| [isWordArt()](#iswordart) | Indicates whether this shape is a word art. Only for the Legacy Shape of xls file. |
| [moveToRange(upperLeftRow, upperLeftColumn, lowerRightRow, lowerRightColumn)](#movetorange) | Moves the shape to a specified range. |
| [removeActiveXControl()](#removeactivexcontrol) | Remove activeX control. |
| [removeHyperlink()](#removehyperlink) | Removes the hyperlink of the shape. |
| [setAlternativeText()](#setalternativetext) | Returns or sets the descriptive (alternative) text string of the Shape object. |
| [setAnchorType()](#setanchortype) | Gets and set the type of the shape anchor placeholder. The value of the property is ShapeAnchorType integer constant. |
| [setAspectRatioLocked()](#setaspectratiolocked) | True means that aspect ratio of the shape is locked. Only for pictures and Ole Objects. |
| [setAutoShapeType()](#setautoshapetype) | Gets and sets the auto shape type. The value of the property is AutoShapeType integer constant. |
| [setBottom()](#setbottom) | Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels. |
| [setCreateId()](#setcreateid) | Gets and sets create id for this shape. |
| [setDecorative()](#setdecorative) |  |
| [setDropDownLines()](#setdropdownlines) | Gets or sets the number of list lines displayed in the drop-down portion of a combo box. |
| [setFilled()](#setfilled) | Indicates whether the fill format is visible. |
| [setFlippedHorizontally()](#setflippedhorizontally) | Gets and sets whether shape is horizontally flipped . |
| [setFlippedVertically()](#setflippedvertically) | Gets and sets whether shape is vertically flipped . |
| [setFont()](#setfont) | Represents the font of shape. |
| [setHasLine()](#sethasline) | Gets and sets the line border of the shape is visible. |
| [setHeight()](#setheight) | Represents the height of shape, in unit of pixel. |
| [setHeightCM()](#setheightcm) | Represents the height of the shape, in unit of centimeters. |
| [setHeightInShape()](#setheightinshape) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the pare |
| [setHeightInch()](#setheightinch) | Represents the height of the shape, in unit of inches. |
| [setHeightPt()](#setheightpt) | Represents the height of the shape, in unit of points. |
| [setHeightScale()](#setheightscale) | Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the Heigh |
| [setHidden()](#sethidden) | Indicates whether the object is visible. |
| [setHtmlText()](#sethtmltext) | Gets and sets the html string which contains data and some formats in this textbox. |
| [setInputRange()](#setinputrange) | Gets or sets the worksheet range used to fill the specified combo box. |
| [setInputRange(formula, isR1C1, isLocal)](#setinputrange-1) | Sets the range used to fill the control. |
| [setLeft()](#setleft) | Represents the horizontal offset of shape from its left column, in unit of pixels. |
| [setLeftCM()](#setleftcm) | Represents the horizontal offset of shape from its left column, in unit of centimeters. |
| [setLeftInShape()](#setleftinshape) | Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the pa |
| [setLeftInch()](#setleftinch) | Represents the horizontal offset of shape from its left column, in unit of inches. |
| [setLeftToCorner()](#setlefttocorner) | Gets and sets the horizonal offset of shape from worksheet left border. |
| [setLinkedCell()](#setlinkedcell) | Gets or sets the worksheet range linked to the control's value. |
| [setLinkedCell(formula, isR1C1, isLocal)](#setlinkedcell-1) | Sets the range linked to the control's value. |
| [setLockAspectRatio()](#setlockaspectratio) | True means that aspect ratio of the shape is locked. Only for pictures and Ole Objects. NOTE: This member is now obsolet |
| [setLocked()](#setlocked) | True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the wo |
| [setLockedProperty(type, value)](#setlockedproperty) | Set the locked property. |
| [setLowerDeltaX()](#setlowerdeltax) | Gets or sets the shape's horizontal offset from its lower right corner column. The range of value is 0 to 1024. |
| [setLowerDeltaY()](#setlowerdeltay) | Gets or sets the shape's vertical offset from its lower right corner row. The range of value is 0 to 256. |
| [setLowerRightColumn()](#setlowerrightcolumn) | Represents lower right corner column index. |
| [setLowerRightRow()](#setlowerrightrow) | Represents lower right corner row index. |
| [setMacroName()](#setmacroname) | Gets and sets the name of macro. |
| [setName()](#setname) | Gets and sets the name of the shape. |
| [setPlacement()](#setplacement) | Represents the way the drawing object is attached to the cells below it. The property controls the placement of an objec |
| [setPrintable()](#setprintable) | Indicates whether the object is printable. If False, this shape will not be printed when printing. |
| [setRelativeToOriginalPictureSize()](#setrelativetooriginalpicturesize) | Indicates whether shape is relative to original picture size. |
| [setRight()](#setright) | Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels. |
| [setRotationAngle()](#setrotationangle) | Gets and sets the rotation of the shape. |
| [setSelectedIndex()](#setselectedindex) | Gets or sets the index number of the currently selected item in a list box or combo box. Zero-based. -1 presents no item |
| [setShadow()](#setshadow) | Indicates whether the combobox has 3-D shading. |
| [setSoftEdges()](#setsoftedges) | Gets and sets the radius of blur to apply to the edges, in unit of points. |
| [setText()](#settext) | Gets and sets the text of this shape. |
| [setTextDirection()](#settextdirection) | Gets/Sets the direction of the text flow for this object. The value of the property is TextDirectionType integer constan |
| [setTextHorizontalAlignment()](#settexthorizontalalignment) | Gets and sets the text horizontal alignment type of the shape. The value of the property is TextAlignmentType integer co |
| [setTextHorizontalOverflow()](#settexthorizontaloverflow) | Gets and sets the text horizontal overflow type of the shape which contains text. The value of the property is TextOverf |
| [setTextOptions()](#settextoptions) | Represents the text options of the shape. |
| [setTextOrientationType()](#settextorientationtype) | Gets and sets the text orientation type of the shape. The value of the property is TextOrientationType integer constant. |
| [setTextShapeType()](#settextshapetype) | Gets and sets the preset text shape type. The value of the property is AutoShapeType integer constant. |
| [setTextVerticalAlignment()](#settextverticalalignment) | Gets and sets the text vertical alignment type of the shape. The value of the property is TextAlignmentType integer cons |
| [setTextVerticalOverflow()](#settextverticaloverflow) | Gets and sets the text vertical overflow type of the shape which contains text. The value of the property is TextOverflo |
| [setTextWrapped()](#settextwrapped) | Gets and sets the text wrapped type of the shape which contains text. |
| [setTitle()](#settitle) | Specifies the title (caption) of the current shape object. |
| [setTop()](#settop) | Represents the vertical offset of shape from its top row, in unit of pixels. If the shape is in the chart, represents th |
| [setTopCM()](#settopcm) | Represents the vertical offset of shape from its top row, in unit of centimeters. |
| [setTopInShape()](#settopinshape) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the pare |
| [setTopInch()](#settopinch) | Represents the vertical offset of shape from its top row, in unit of inches. |
| [setTopToCorner()](#settoptocorner) | Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels. |
| [setUpperDeltaX()](#setupperdeltax) | Gets or sets the shape's horizontal offset from its upper left corner column. The range of value is 0 to 1024. |
| [setUpperDeltaY()](#setupperdeltay) | Gets or sets the shape's vertical offset from its upper left corner row. The range of value is 0 to 256. |
| [setUpperLeftColumn()](#setupperleftcolumn) | Represents upper left corner column index. |
| [setUpperLeftRow()](#setupperleftrow) | Represents the top row index. If the shape is in the shape or in the group , UpperLeftRow will be ignored. |
| [setWidth()](#setwidth) | Represents the width of shape, in unit of pixels. |
| [setWidthCM()](#setwidthcm) | Represents the width of the shape, in unit of centimeters. |
| [setWidthInShape()](#setwidthinshape) | Represents the width of the shape, in unit of 1/4000 of the parent shape. Only Applies when this shape in the group or c |
| [setWidthInch()](#setwidthinch) | Represents the width of the shape, in unit of inch. |
| [setWidthPt()](#setwidthpt) | Represents the width of the shape, in unit of point. |
| [setWidthScale()](#setwidthscale) | Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthS |
| [setX()](#setx) | Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels. |
| [setY()](#sety) | Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels. |
| [setZOrderPosition()](#setzorderposition) | Returns the position of a shape in the z-order. |
| [toFrontOrBack(orders)](#tofrontorback) | Brings the shape to the front or sends the shape to back. |
| [toImage()](#toimage) | Saves the shape to a file. |
| [updateSelectedValue()](#updateselectedvalue) | Update the selected value by the value of the linked cell. |

### addHyperlink(address) {#addhyperlink}

Adds a hyperlink to the shape.

| Parameter | Type | Description |
| --- | --- | --- |
| address | String | Address of the hyperlink. |

**Returns:** Hyperlink — `Hyperlink` Return the new hyperlink object.

### alignTopRightCorner(topRow, rightColumn) {#aligntoprightcorner}

Moves the picture to the top-right corner.

| Parameter | Type | Description |
| --- | --- | --- |
| topRow | Number | the row index. |
| rightColumn | Number | the column index. |

### calculateTextSize() {#calculatetextsize}

Recalculate the text area

**Returns:** Array of Number — `Array of Number` Text's Size in an array(width and height).

### characters(startIndex, length) {#characters}

Returns a Characters object that represents a range of characters within the text. This method only works on shape with title.

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Number | The index of the start of the character. |
| length | Number | The number of characters. |

**Returns:** FontSetting — `FontSetting` Characters object.

### fitToTextSize() {#fittotextsize}

### formatCharacters(startIndex, length, font, flag) {#formatcharacters}

Formats some characters with the font setting.

| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | Number | The start index. |
| length | Number | The length. |
| font | Font | The font setting. |
| flag | StyleFlag | The flag of the font setting. |

### getActualBox() {#getactualbox}

Get the actual position and size of the shape (after applying rotation, flip, etc.) Note:The interface is not fully functional, especially the location information is not correct.It is recommended not to use this interface until the function is complete.@return {float[]} Return the position and size in the order of x, y, w, h

### getActualLowerRightRow() {#getactuallowerrightrow}

Get the actual bottom row.

### getAlternativeText() {#getalternativetext}

Returns or sets the descriptive (alternative) text string of the Shape object.

### getAnchorType() {#getanchortype}

Gets and set the type of the shape anchor placeholder. The value of the property is ShapeAnchorType integer constant.

### getAutoShapeType() {#getautoshapetype}

Gets and sets the auto shape type. The value of the property is AutoShapeType integer constant.

### getBottom() {#getbottom}

Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels.

### getCharacters() {#getcharacters}

Returns all Characters objects that represents a range of characters within the text . NOTE: This method is now obsolete. Instead, please use Shape.GetRichFormattings() method. This method will be removed 12 months later since November 2023. Aspose apologizes for any inconvenience you may have experienced.

**Returns:** ArrayList — `ArrayList` All Characters objects

### getConnectionPoints() {#getconnectionpoints}

Get the connection points

**Returns:** Array of Array of float — `Array of Array of float` [X,Y] pairs of the connection point. Every item is a float[2] array, [0] represents x and [1] represents y.

### getControlData() {#getcontroldata}

Gets the data of control.

### getCreateId() {#getcreateid}

Gets and sets create id for this shape.

### getDropDownLines() {#getdropdownlines}

Gets or sets the number of list lines displayed in the drop-down portion of a combo box.

### getFill() {#getfill}

Returns a FillFormat object that contains fill formatting properties for the specified shape.

### getFillFormat() {#getfillformat}

Returns a MsoFillFormat object that contains fill formatting properties for the specified shape. NOTE: This member is now obsolete. Instead, please use Shape.Fill property. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

### getFont() {#getfont}

Represents the font of shape.

### getFormatPicture() {#getformatpicture}

Gets and sets the options of the picture format.

### getGeometry() {#getgeometry}

Gets the geometry

### getGlow() {#getglow}

Represents a GlowEffect object that specifies glow effect for the chart element or shape.

### getGroup() {#getgroup}

Gets the group shape which contains this shape.

### getHeight() {#getheight}

Represents the height of shape, in unit of pixel.

### getHeightCM() {#getheightcm}

Represents the height of the shape, in unit of centimeters.

### getHeightInShape() {#getheightinshape}

Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. Only Applies when this shape in the group or chart.

### getHeightInch() {#getheightinch}

Represents the height of the shape, in unit of inches.

### getHeightPt() {#getheightpt}

Represents the height of the shape, in unit of points.

### getHeightScale() {#getheightscale}

Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100;

### getHtmlText() {#gethtmltext}

Gets and sets the html string which contains data and some formats in this textbox.

### getHyperlink() {#gethyperlink}

Gets the hyperlink of the shape.

### getId() {#getid}

Gets the identifier of this shape.

### getInputRange() {#getinputrange}

Gets or sets the worksheet range used to fill the specified combo box.

### getInputRange(isR1C1, isLocal) {#getinputrange-1}

Gets the range used to fill the control.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns:** String — `String` The range used to fill the control.

### getLeft() {#getleft}

Represents the horizontal offset of shape from its left column, in unit of pixels.

### getLeftCM() {#getleftcm}

Represents the horizontal offset of shape from its left column, in unit of centimeters.

### getLeftInShape() {#getleftinshape}

Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. Only Applies when this shape in the group or chart.

### getLeftInch() {#getleftinch}

Represents the horizontal offset of shape from its left column, in unit of inches.

### getLeftToCorner() {#getlefttocorner}

Gets and sets the horizonal offset of shape from worksheet left border.

### getLine() {#getline}

Gets line style

### getLineFormat() {#getlineformat}

Returns a MsoLineFormat object that contains line formatting properties for the specified shape. NOTE: This member is now obsolete. Instead, please use Shape.Line property. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

### getLinkedCell() {#getlinkedcell}

Gets or sets the worksheet range linked to the control's value.

### getLinkedCell(isR1C1, isLocal) {#getlinkedcell-1}

Gets the range linked to the control's value.

| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns:** String — `String` The range linked to the control's value.

### getLockedProperty(type) {#getlockedproperty}

Gets the value of locked property.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | ShapeLockType |

**Returns:** boolean — `boolean` Returns the value of locked property.

### getLowerDeltaX() {#getlowerdeltax}

Gets or sets the shape's horizontal offset from its lower right corner column. The range of value is 0 to 1024.

### getLowerDeltaY() {#getlowerdeltay}

Gets or sets the shape's vertical offset from its lower right corner row. The range of value is 0 to 256.

### getLowerRightColumn() {#getlowerrightcolumn}

Represents lower right corner column index.

### getLowerRightRow() {#getlowerrightrow}

Represents lower right corner row index.

### getMacroName() {#getmacroname}

Gets and sets the name of macro.

### getMsoDrawingType() {#getmsodrawingtype}

Gets drawing type. The value of the property is MsoDrawingType integer constant.

### getName() {#getname}

Gets and sets the name of the shape.

### getPaths() {#getpaths}

Gets the paths of a custom geometric shape.

### getPlacement() {#getplacement}

Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. The value of the property is PlacementType integer constant.

### getReflection() {#getreflection}

Represents a ReflectionEffect object that specifies reflection effect for the chart element or shape.

### getRelativeToOriginalPictureSize() {#getrelativetooriginalpicturesize}

Indicates whether shape is relative to original picture size.

### getResultOfSmartArt() {#getresultofsmartart}

Converting smart art to grouped shapes.

### getRichFormattings() {#getrichformattings}

Returns all Characters objects that represents a range of characters within the text .

**Returns:** Array ofFontSetting — `Array ofFontSetting` All Characters objects

### getRight() {#getright}

Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels.

### getRotationAngle() {#getrotationangle}

Gets and sets the rotation of the shape.

### getSelectedCell() {#getselectedcell}

Gets the selected cell in the input range of the combo box.

### getSelectedIndex() {#getselectedindex}

Gets or sets the index number of the currently selected item in a list box or combo box. Zero-based. -1 presents no item is selected.

### getSelectedValue() {#getselectedvalue}

Gets the selected value of the combox box.

### getShadow() {#getshadow}

Indicates whether the combobox has 3-D shading.

### getShadowEffect() {#getshadoweffect}

Represents a ShadowEffect object that specifies shadow effect for the chart element or shape.

### getSoftEdges() {#getsoftedges}

Gets and sets the radius of blur to apply to the edges, in unit of points.

### getSpid() {#getspid}

Specifies an optional string identifier that an application can use to identify the particular shape.

### getSpt() {#getspt}

Specifies an optional number that an application can use to associate the particular shape with a defined shape type.

### getText() {#gettext}

Gets and sets the text of this shape.

### getTextBody() {#gettextbody}

Gets and sets the setting of the shape's text.

### getTextBoxOptions() {#gettextboxoptions}

### getTextDirection() {#gettextdirection}

Gets/Sets the direction of the text flow for this object. The value of the property is TextDirectionType integer constant.

### getTextEffect() {#gettexteffect}

Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape. Applies to Shape objects that represent WordArt.

### getTextHorizontalAlignment() {#gettexthorizontalalignment}

Gets and sets the text horizontal alignment type of the shape. The value of the property is TextAlignmentType integer constant.

### getTextHorizontalOverflow() {#gettexthorizontaloverflow}

Gets and sets the text horizontal overflow type of the shape which contains text. The value of the property is TextOverflowType integer constant.

### getTextOptions() {#gettextoptions}

Represents the text options of the shape.

### getTextOrientationType() {#gettextorientationtype}

Gets and sets the text orientation type of the shape. The value of the property is TextOrientationType integer constant.

### getTextShapeType() {#gettextshapetype}

Gets and sets the preset text shape type. The value of the property is AutoShapeType integer constant.

### getTextVerticalAlignment() {#gettextverticalalignment}

Gets and sets the text vertical alignment type of the shape. The value of the property is TextAlignmentType integer constant.

### getTextVerticalOverflow() {#gettextverticaloverflow}

Gets and sets the text vertical overflow type of the shape which contains text. The value of the property is TextOverflowType integer constant.

### getThreeDFormat() {#getthreedformat}

Gets and sets 3d format of the shape.

### getTitle() {#gettitle}

Specifies the title (caption) of the current shape object.

### getTop() {#gettop}

Represents the vertical offset of shape from its top row, in unit of pixels. If the shape is in the chart, represents the vertical offset of shape from its top border.

### getTopCM() {#gettopcm}

Represents the vertical offset of shape from its top row, in unit of centimeters.

### getTopInShape() {#gettopinshape}

Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. Only Applies when this shape in the group or chart.

### getTopInch() {#gettopinch}

Represents the vertical offset of shape from its top row, in unit of inches.

### getTopToCorner() {#gettoptocorner}

Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels.

### getType() {#gettype}

Gets the auto shape type. The value of the property is AutoShapeType integer constant.

### getUpperDeltaX() {#getupperdeltax}

Gets or sets the shape's horizontal offset from its upper left corner column. The range of value is 0 to 1024.

### getUpperDeltaY() {#getupperdeltay}

Gets or sets the shape's vertical offset from its upper left corner row. The range of value is 0 to 256.

### getUpperLeftColumn() {#getupperleftcolumn}

Represents upper left corner column index.

### getUpperLeftRow() {#getupperleftrow}

Represents the top row index. If the shape is in the shape or in the group , UpperLeftRow will be ignored.

### getWidth() {#getwidth}

Represents the width of shape, in unit of pixels.

### getWidthCM() {#getwidthcm}

Represents the width of the shape, in unit of centimeters.

### getWidthInShape() {#getwidthinshape}

Represents the width of the shape, in unit of 1/4000 of the parent shape. Only Applies when this shape in the group or chart.

### getWidthInch() {#getwidthinch}

Represents the width of the shape, in unit of inch.

### getWidthPt() {#getwidthpt}

Represents the width of the shape, in unit of point.

### getWidthScale() {#getwidthscale}

Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100;

### getWorksheet() {#getworksheet}

Gets the Worksheet object which contains this shape.

### getX() {#getx}

Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels.

### getY() {#gety}

Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels.

### getZOrderPosition() {#getzorderposition}

Returns the position of a shape in the z-order.

### hasLine() {#hasline}

Gets and sets the line border of the shape is visible.

### isAspectRatioLocked() {#isaspectratiolocked}

True means that aspect ratio of the shape is locked. Only for pictures and Ole Objects.

### isDecorative() {#isdecorative}

### isEquation() {#isequation}

Indicates whether the shape only contains an equation.

### isFilled() {#isfilled}

Indicates whether the fill format is visible.

### isFlippedHorizontally() {#isflippedhorizontally}

Gets and sets whether shape is horizontally flipped .

### isFlippedVertically() {#isflippedvertically}

Gets and sets whether shape is vertically flipped .

### isGroup() {#isgroup}

Indicates whether this shape is a group shape.

### isHidden() {#ishidden}

Indicates whether the object is visible.

### isInGroup() {#isingroup}

Indicates whether the shape is grouped.

### isLockAspectRatio() {#islockaspectratio}

True means that aspect ratio of the shape is locked. Only for pictures and Ole Objects. NOTE: This member is now obsolete. Instead, please use Shape.IsAspectRatioLocked property. This property will be removed 12 months later since July 2024. Aspose apologizes for any inconvenience you may have experienced.

### isLocked() {#islocked}

True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected.

### isPrintable() {#isprintable}

Indicates whether the object is printable. If False, this shape will not be printed when printing.

### isRichText() {#isrichtext}

Whether or not the text is rich text.

### isSameSetting(obj) {#issamesetting}

Returns whether the shape is same.

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object |  |

**Returns:** boolean — `boolean`

### isSmartArt() {#issmartart}

Indicates whether the shape is a smart art. Only for ooxml file.

### isTextWrapped() {#istextwrapped}

Gets and sets the text wrapped type of the shape which contains text.

### isWordArt() {#iswordart}

Indicates whether this shape is a word art. Only for the Legacy Shape of xls file.

### moveToRange(upperLeftRow, upperLeftColumn, lowerRightRow, lowerRightColumn) {#movetorange}

Moves the shape to a specified range.

| Parameter | Description |
| --- | --- |
| upperLeftRow | Upper left row index. |
| upperLeftColumn | Upper left column index. |
| lowerRightRow | Lower right row index |
| lowerRightColumn | Lower right column index |

### removeActiveXControl() {#removeactivexcontrol}

Remove activeX control.

### removeHyperlink() {#removehyperlink}

Removes the hyperlink of the shape.

### setAlternativeText() {#setalternativetext}

Returns or sets the descriptive (alternative) text string of the Shape object.

### setAnchorType() {#setanchortype}

Gets and set the type of the shape anchor placeholder. The value of the property is ShapeAnchorType integer constant.

### setAspectRatioLocked() {#setaspectratiolocked}

True means that aspect ratio of the shape is locked. Only for pictures and Ole Objects.

### setAutoShapeType() {#setautoshapetype}

Gets and sets the auto shape type. The value of the property is AutoShapeType integer constant.

### setBottom() {#setbottom}

Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels.

### setCreateId() {#setcreateid}

Gets and sets create id for this shape.

### setDecorative() {#setdecorative}

### setDropDownLines() {#setdropdownlines}

Gets or sets the number of list lines displayed in the drop-down portion of a combo box.

### setFilled() {#setfilled}

Indicates whether the fill format is visible.

### setFlippedHorizontally() {#setflippedhorizontally}

Gets and sets whether shape is horizontally flipped .

### setFlippedVertically() {#setflippedvertically}

Gets and sets whether shape is vertically flipped .

### setFont() {#setfont}

Represents the font of shape.

### setHasLine() {#sethasline}

Gets and sets the line border of the shape is visible.

### setHeight() {#setheight}

Represents the height of shape, in unit of pixel.

### setHeightCM() {#setheightcm}

Represents the height of the shape, in unit of centimeters.

### setHeightInShape() {#setheightinshape}

Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. Only Applies when this shape in the group or chart.

### setHeightInch() {#setheightinch}

Represents the height of the shape, in unit of inches.

### setHeightPt() {#setheightpt}

Represents the height of the shape, in unit of points.

### setHeightScale() {#setheightscale}

Gets and sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100;

### setHidden() {#sethidden}

Indicates whether the object is visible.

### setHtmlText() {#sethtmltext}

Gets and sets the html string which contains data and some formats in this textbox.

### setInputRange() {#setinputrange}

Gets or sets the worksheet range used to fill the specified combo box.

### setInputRange(formula, isR1C1, isLocal) {#setinputrange-1}

Sets the range used to fill the control.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The range used to fill the control. |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

### setLeft() {#setleft}

Represents the horizontal offset of shape from its left column, in unit of pixels.

### setLeftCM() {#setleftcm}

Represents the horizontal offset of shape from its left column, in unit of centimeters.

### setLeftInShape() {#setleftinshape}

Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. Only Applies when this shape in the group or chart.

### setLeftInch() {#setleftinch}

Represents the horizontal offset of shape from its left column, in unit of inches.

### setLeftToCorner() {#setlefttocorner}

Gets and sets the horizonal offset of shape from worksheet left border.

### setLinkedCell() {#setlinkedcell}

Gets or sets the worksheet range linked to the control's value.

### setLinkedCell(formula, isR1C1, isLocal) {#setlinkedcell-1}

Sets the range linked to the control's value.

| Parameter | Type | Description |
| --- | --- | --- |
| formula | String | The range linked to the control's value. |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

### setLockAspectRatio() {#setlockaspectratio}

True means that aspect ratio of the shape is locked. Only for pictures and Ole Objects. NOTE: This member is now obsolete. Instead, please use Shape.IsAspectRatioLocked property. This property will be removed 12 months later since July 2024. Aspose apologizes for any inconvenience you may have experienced.

### setLocked() {#setlocked}

True means the object can not be modified when the sheet is protected. Note that this value is meaningful only if the worksheet or objects in the worksheet are protected.

### setLockedProperty(type, value) {#setlockedproperty}

Set the locked property.

| Parameter | Type | Description |
| --- | --- | --- |
| type | Number | ShapeLockType |
| value | boolean | The value of the property. |

### setLowerDeltaX() {#setlowerdeltax}

Gets or sets the shape's horizontal offset from its lower right corner column. The range of value is 0 to 1024.

### setLowerDeltaY() {#setlowerdeltay}

Gets or sets the shape's vertical offset from its lower right corner row. The range of value is 0 to 256.

### setLowerRightColumn() {#setlowerrightcolumn}

Represents lower right corner column index.

### setLowerRightRow() {#setlowerrightrow}

Represents lower right corner row index.

### setMacroName() {#setmacroname}

Gets and sets the name of macro.

### setName() {#setname}

Gets and sets the name of the shape.

### setPlacement() {#setplacement}

Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. The value of the property is PlacementType integer constant.

### setPrintable() {#setprintable}

Indicates whether the object is printable. If False, this shape will not be printed when printing.

### setRelativeToOriginalPictureSize() {#setrelativetooriginalpicturesize}

Indicates whether shape is relative to original picture size.

### setRight() {#setright}

Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels.

### setRotationAngle() {#setrotationangle}

Gets and sets the rotation of the shape.

### setSelectedIndex() {#setselectedindex}

Gets or sets the index number of the currently selected item in a list box or combo box. Zero-based. -1 presents no item is selected.

### setShadow() {#setshadow}

Indicates whether the combobox has 3-D shading.

### setSoftEdges() {#setsoftedges}

Gets and sets the radius of blur to apply to the edges, in unit of points.

### setText() {#settext}

Gets and sets the text of this shape.

### setTextDirection() {#settextdirection}

Gets/Sets the direction of the text flow for this object. The value of the property is TextDirectionType integer constant.

### setTextHorizontalAlignment() {#settexthorizontalalignment}

Gets and sets the text horizontal alignment type of the shape. The value of the property is TextAlignmentType integer constant.

### setTextHorizontalOverflow() {#settexthorizontaloverflow}

Gets and sets the text horizontal overflow type of the shape which contains text. The value of the property is TextOverflowType integer constant.

### setTextOptions() {#settextoptions}

Represents the text options of the shape.

### setTextOrientationType() {#settextorientationtype}

Gets and sets the text orientation type of the shape. The value of the property is TextOrientationType integer constant.

### setTextShapeType() {#settextshapetype}

Gets and sets the preset text shape type. The value of the property is AutoShapeType integer constant.

### setTextVerticalAlignment() {#settextverticalalignment}

Gets and sets the text vertical alignment type of the shape. The value of the property is TextAlignmentType integer constant.

### setTextVerticalOverflow() {#settextverticaloverflow}

Gets and sets the text vertical overflow type of the shape which contains text. The value of the property is TextOverflowType integer constant.

### setTextWrapped() {#settextwrapped}

Gets and sets the text wrapped type of the shape which contains text.

### setTitle() {#settitle}

Specifies the title (caption) of the current shape object.

### setTop() {#settop}

Represents the vertical offset of shape from its top row, in unit of pixels. If the shape is in the chart, represents the vertical offset of shape from its top border.

### setTopCM() {#settopcm}

Represents the vertical offset of shape from its top row, in unit of centimeters.

### setTopInShape() {#settopinshape}

Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. Only Applies when this shape in the group or chart.

### setTopInch() {#settopinch}

Represents the vertical offset of shape from its top row, in unit of inches.

### setTopToCorner() {#settoptocorner}

Gets and sets the vertical offset of shape from worksheet top border, in unit of pixels.

### setUpperDeltaX() {#setupperdeltax}

Gets or sets the shape's horizontal offset from its upper left corner column. The range of value is 0 to 1024.

### setUpperDeltaY() {#setupperdeltay}

Gets or sets the shape's vertical offset from its upper left corner row. The range of value is 0 to 256.

### setUpperLeftColumn() {#setupperleftcolumn}

Represents upper left corner column index.

### setUpperLeftRow() {#setupperleftrow}

Represents the top row index. If the shape is in the shape or in the group , UpperLeftRow will be ignored.

### setWidth() {#setwidth}

Represents the width of shape, in unit of pixels.

### setWidthCM() {#setwidthcm}

Represents the width of the shape, in unit of centimeters.

### setWidthInShape() {#setwidthinshape}

Represents the width of the shape, in unit of 1/4000 of the parent shape. Only Applies when this shape in the group or chart.

### setWidthInch() {#setwidthinch}

Represents the width of the shape, in unit of inch.

### setWidthPt() {#setwidthpt}

Represents the width of the shape, in unit of point.

### setWidthScale() {#setwidthscale}

Gets and sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100;

### setX() {#setx}

Gets and sets the horizontal offset of shape from worksheet left border,in unit of pixels.

### setY() {#sety}

Gets and sets the vertical offset of shape from worksheet top border,in unit of pixels.

### setZOrderPosition() {#setzorderposition}

Returns the position of a shape in the z-order.

### toFrontOrBack(orders) {#tofrontorback}

Brings the shape to the front or sends the shape to back.

| Parameter | Type | Description |
| --- | --- | --- |
| orders | Number | If it's less than zero, sets the shape to back. If it's greater than zero, brings the shape to front. |

### toImage() {#toimage}

Saves the shape to a file.

### updateSelectedValue() {#updateselectedvalue}

Update the selected value by the value of the linked cell.
