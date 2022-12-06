---
title: CommentShape
second_title: Aspose.Cells for Java API Reference
description: Represents the shape of the comment.
type: docs
url: /java/com.aspose.cells/commentshape/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Shape](../../com.aspose.cells/shape)
```
public class CommentShape extends Shape
```

Represents the shape of the comment.

```
//source file
         String fileName = "";
 
         //Instantiating a Workbook object
         Workbook workbook = new Workbook(fileName);
 
         ShapeCollection shapes = workbook.getWorksheets().get(0).getShapes();
 
         //Check if a shape is CommentShape
         CommentShape commentShape = null;
         if (shapes.get(0).getMsoDrawingType() == com.aspose.cells.MsoDrawingType.COMMENT)
         {
             //Represents the shape of the comment.
             commentShape = (CommentShape)shapes.get(0);
         }
 
         //do your business
```
## Methods

| Method | Description |
| --- | --- |
| [addHyperlink(String address)](#addHyperlink-java.lang.String-) | Adds a hyperlink to the shape. |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | Moves the picture to the top-right corner. |
| [calculateTextSize()](#calculateTextSize--) | Recalculate the text area |
| [characters(int startIndex, int length)](#characters-int-int-) | Returns a Characters object that represents a range of characters within the text. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [formatCharacters(int startIndex, int length, Font font)](#formatCharacters-int-int-com.aspose.cells.Font-) | Formats some characters with the font setting. |
| [formatCharacters(int startIndex, int length, Font font, StyleFlag flag)](#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Formats some characters with the font setting. |
| [getActiveXControl()](#getActiveXControl--) | Gets the ActiveX control. |
| [getActualLowerRightRow()](#getActualLowerRightRow--) | Get the actual bottom row. |
| [getAlternativeText()](#getAlternativeText--) | Returns or sets the descriptive (alternative) text string of the [Shape](../../com.aspose.cells/shape) object. |
| [getAnchorType()](#getAnchorType--) | the shape anchor placeholder. |
| [getAutoShapeType()](#getAutoShapeType--) | the auto shape type. |
| [getBottom()](#getBottom--) | Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels. |
| [getCharacters()](#getCharacters--) | Returns all Characters objects that represents a range of characters within the text . |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | Gets the comment object. |
| [getConnectionPoints()](#getConnectionPoints--) | Get the connection points |
| [getControlData()](#getControlData--) | Gets the data of control. |
| [getCreateId()](#getCreateId--) | create id for this shape. |
| [getFill()](#getFill--) | Returns a [Area.getFillFormat()](../../com.aspose.cells/area\#getFillFormat--) object that contains fill formatting properties for the specified shape. |
| [getFillFormat()](#getFillFormat--) | Returns a MsoFillFormat object that contains fill formatting properties for the specified shape. |
| [getFont()](#getFont--) | Represents the font of shape. |
| [getFormat()](#getFormat--) | Represents the setting of the shape's formatting. |
| [getFormatPicture()](#getFormatPicture--) | the options of the picture format. |
| [getGeometry()](#getGeometry--) | Gets the geometry |
| [getGlow()](#getGlow--) | Represents a [ShapeFormat.getGlowEffect()](../../com.aspose.cells/shapeformat\#getGlowEffect--) object that specifies glow effect for the chart element or shape. |
| [getGroup()](#getGroup--) | Gets the group shape which contains this shape. |
| [getHeight()](#getHeight--) | Represents the height of shape, in unit of pixel. |
| [getHeightCM()](#getHeightCM--) | Represents the height of the shape, in unit of centimeters. |
| [getHeightInChart()](#getHeightInChart--) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. |
| [getHeightInShape()](#getHeightInShape--) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. |
| [getHeightInch()](#getHeightInch--) | Represents the height of the shape, in unit of inches. |
| [getHeightPt()](#getHeightPt--) | Represents the height of the shape, in unit of points. |
| [getHeightScale()](#getHeightScale--) | the height scale,in unit of percent of the original picture height. |
| [getHtmlText()](#getHtmlText--) | the html string which contains data and some formats in this textbox. |
| [getHyperlink()](#getHyperlink--) | Gets the hyperlink of the shape. |
| [getId()](#getId--) | Gets the identifier of this shape. |
| [getInputRange()](#getInputRange--) | the worksheet range used to fill the specified combo box. |
| [getInputRange(boolean isR1C1, boolean isLocal)](#getInputRange-boolean-boolean-) | Gets the range used to fill the control. |
| [getLeft()](#getLeft--) | Represents the horizontal offset of shape from its left column, in unit of pixels. |
| [getLeftCM()](#getLeftCM--) | Represents the horizontal offset of shape from its left column, in unit of centimeters. |
| [getLeftInChart()](#getLeftInChart--) | Represents the vertical offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. |
| [getLeftInShape()](#getLeftInShape--) | Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. |
| [getLeftInch()](#getLeftInch--) | Represents the horizontal offset of shape from its left column, in unit of inches. |
| [getLeftToCorner()](#getLeftToCorner--) | the horizonal offset of shape from worksheet left border. |
| [getLine()](#getLine--) | Gets line style |
| [getLineFormat()](#getLineFormat--) | Returns a MsoLineFormat object that contains line formatting properties for the specified shape. |
| [getLinkedCell()](#getLinkedCell--) | the worksheet range linked to the control's value. |
| [getLinkedCell(boolean isR1C1, boolean isLocal)](#getLinkedCell-boolean-boolean-) | Gets the range linked to the control's value. |
| [getLockedProperty(int type)](#getLockedProperty-int-) | Gets the value of locked property. |
| [getLowerDeltaX()](#getLowerDeltaX--) | the shape's horizontal offset from its lower right corner column. |
| [getLowerDeltaY()](#getLowerDeltaY--) | the shape's vertical offset from its lower right corner row. |
| [getLowerRightColumn()](#getLowerRightColumn--) | Represents lower right corner column index. |
| [getLowerRightRow()](#getLowerRightRow--) | Represents lower right corner row index. |
| [getMacroName()](#getMacroName--) | the name of macro. |
| [getMsoDrawingType()](#getMsoDrawingType--) | Gets mso drawing type. |
| [getName()](#getName--) | the name of the shape. |
| [getPaths()](#getPaths--) | Gets the paths of a custom geometric shape. |
| [getPlacement()](#getPlacement--) | Represents the way the drawing object is attached to the cells below it. |
| [getPositionX()](#getPositionX--) | the horizonal offset of shape from worksheet left border,in unit of pixels. |
| [getPositionY()](#getPositionY--) | the vertical offset of shape from worksheet top border,in unit of pixels. |
| [getReflection()](#getReflection--) | Represents a [ReflectionEffect](../../com.aspose.cells/reflectioneffect) object that specifies reflection effect for the chart element or shape. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | Indicates whether shape is relative to original picture size. |
| [getResultOfSmartArt()](#getResultOfSmartArt--) | Converting smart art to grouped shapes. |
| [getRight()](#getRight--) | Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels. |
| [getRotationAngle()](#getRotationAngle--) | the rotation of the shape. |
| [getShadowEffect()](#getShadowEffect--) | Represents a [ShadowEffect](../../com.aspose.cells/shadoweffect) object that specifies shadow effect for the chart element or shape. |
| [getSoftEdges()](#getSoftEdges--) | the radius of blur to apply to the edges, in unit of points. |
| [getSpid()](#getSpid--) | Specifies an optional string that an application can use to Identify the particular shape. |
| [getSpt()](#getSpt--) | Specifies an optional number that an application can use to associate the particular shape with a defined shape type. |
| [getText()](#getText--) | Represents the string in this TextBox object. |
| [getTextBody()](#getTextBody--) | the setting of the shape's text. |
| [getTextDirection()](#getTextDirection--) | Gets/Sets the direction of the text flow for this object. |
| [getTextEffect()](#getTextEffect--) | Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape. |
| [getTextFrame()](#getTextFrame--) | Returns a TextFrame object that contains the alignment and anchoring properties for the specified shape. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | the text horizontal alignment type of the shape. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | the text horizontal overflow type of the shape which contains text. |
| [getTextOptions()](#getTextOptions--) | Represents the text options of the shape. |
| [getTextOrientationType()](#getTextOrientationType--) | the text orientation type of the shape. |
| [getTextShapeType()](#getTextShapeType--) | the preset text shape type. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | the text vertical alignment type of the shape. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | the text vertical overflow type of the shape which contains text. |
| [getThreeDFormat()](#getThreeDFormat--) | 3d format of the shape. |
| [getTitle()](#getTitle--) | Specifies the title (caption) of the current shape object. |
| [getTop()](#getTop--) | Represents the vertical offset of shape from its top row, in unit of pixels. |
| [getTopCM()](#getTopCM--) | Represents the vertical offset of shape from its top row, in unit of centimeters. |
| [getTopInChart()](#getTopInChart--) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. |
| [getTopInShape()](#getTopInShape--) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. |
| [getTopInch()](#getTopInch--) | Represents the vertical offset of shape from its top row, in unit of inches. |
| [getTopToCorner()](#getTopToCorner--) | the vertical offset of shape from worksheet top border, in unit of pixels. |
| [getType()](#getType--) | Gets the auto shape type. |
| [getUpperDeltaX()](#getUpperDeltaX--) | the shape's horizontal offset from its upper left corner column. |
| [getUpperDeltaY()](#getUpperDeltaY--) | the shape's vertical offset from its upper left corner row. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Represents upper left corner column index. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Represents upper left corner row index. |
| [getWidth()](#getWidth--) | Represents the width of shape, in unit of pixels. |
| [getWidthCM()](#getWidthCM--) | Represents the width of the shape, in unit of centimeters. |
| [getWidthInChart()](#getWidthInChart--) | Represents the width of the shape, in unit of 1/4000 of the parent shape. |
| [getWidthInShape()](#getWidthInShape--) | Represents the width of the shape, in unit of 1/4000 of the parent shape. |
| [getWidthInch()](#getWidthInch--) | Represents the width of the shape, in unit of inch. |
| [getWidthPt()](#getWidthPt--) | Represents the width of the shape, in unit of point. |
| [getWidthScale()](#getWidthScale--) | the width scale, in unit of percent of the original picture width. |
| [getWorksheet()](#getWorksheet--) | Gets the [Range.getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) object which contains this shape. |
| [getX()](#getX--) | the horizontal offset of shape from worksheet left border,in unit of pixels. |
| [getY()](#getY--) | the vertical offset of shape from worksheet top border,in unit of pixels. |
| [getZOrderPosition()](#getZOrderPosition--) | Returns the position of a shape in the z-order. |
| [hasLine()](#hasLine--) | the line border of the shape is visible. |
| [hashCode()](#hashCode--) |  |
| [isEquation()](#isEquation--) | Indicates whether the shape only contains an equation. |
| [isFilled()](#isFilled--) | Indicates whether the fill format is visible. |
| [isFlippedHorizontally()](#isFlippedHorizontally--) | whether shape is horizontally flipped . |
| [isFlippedVertically()](#isFlippedVertically--) | whether shape is vertically flipped . |
| [isGroup()](#isGroup--) | Indicates whether the shape is a group. |
| [isHidden()](#isHidden--) | Indicates whether the object is visible. |
| [isInGroup()](#isInGroup--) | Indicates whether the shape is grouped. |
| [isLockAspectRatio()](#isLockAspectRatio--) | True means that don't allow changes in aspect ratio. |
| [isLocked()](#isLocked--) | True if the object is locked, False if the object can be modified when the sheet is protected. |
| [isPrintable()](#isPrintable--) | True if the object is printable |
| [isRichText()](#isRichText--) | Whether or not the text is rich text. |
| [isSameSetting(Object obj)](#isSameSetting-java.lang.Object-) | Returns whether the shape is same. |
| [isSmartArt()](#isSmartArt--) | Indicates whether the shape is smart art. |
| [isTextWrapped()](#isTextWrapped--) | the text wrapped type of the shape which contains text. |
| [isWordArt()](#isWordArt--) | Indicates whether this shape is a word art. |
| [moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)](#moveToRange-int-int-int-int-) | Moves the shape to a specified range. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeActiveXControl()](#removeActiveXControl--) | Remove activeX control. |
| [removeHyperlink()](#removeHyperlink--) | Remove the hyperlink of the shape. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | For the description of this property, please see [getAlternativeText()](../../com.aspose.cells/shape\#getAlternativeText--) |
| [setAnchorType(int value)](#setAnchorType-int-) | For the description of this property, please see [getAnchorType()](../../com.aspose.cells/shape\#getAnchorType--) |
| [setAutoShapeType(int value)](#setAutoShapeType-int-) | For the description of this property, please see [getAutoShapeType()](../../com.aspose.cells/shape\#getAutoShapeType--) |
| [setBottom(int value)](#setBottom-int-) | For the description of this property, please see [getBottom()](../../com.aspose.cells/shape\#getBottom--) |
| [setCreateId(UUID value)](#setCreateId-java.util.UUID-) | For the description of this property, please see [getCreateId()](../../com.aspose.cells/shape\#getCreateId--) |
| [setFilled(boolean value)](#setFilled-boolean-) | For the description of this property, please see [isFilled()](../../com.aspose.cells/shape\#isFilled--) |
| [setFlippedHorizontally(boolean value)](#setFlippedHorizontally-boolean-) | For the description of this property, please see [isFlippedHorizontally()](../../com.aspose.cells/shape\#isFlippedHorizontally--) |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | For the description of this property, please see [isFlippedVertically()](../../com.aspose.cells/shape\#isFlippedVertically--) |
| [setFont(Font value)](#setFont-com.aspose.cells.Font-) | For the description of this property, please see [getFont()](../../com.aspose.cells/shape\#getFont--) |
| [setHasLine(boolean value)](#setHasLine-boolean-) | For the description of this property, please see [hasLine()](../../com.aspose.cells/shape\#hasLine--) |
| [setHeight(int value)](#setHeight-int-) | For the description of this property, please see [getHeight()](../../com.aspose.cells/shape\#getHeight--) |
| [setHeightCM(double value)](#setHeightCM-double-) | For the description of this property, please see [getHeightCM()](../../com.aspose.cells/shape\#getHeightCM--) |
| [setHeightInChart(int value)](#setHeightInChart-int-) | For the description of this property, please see [getHeightInChart()](../../com.aspose.cells/shape\#getHeightInChart--) |
| [setHeightInShape(int value)](#setHeightInShape-int-) | For the description of this property, please see [getHeightInShape()](../../com.aspose.cells/shape\#getHeightInShape--) |
| [setHeightInch(double value)](#setHeightInch-double-) | For the description of this property, please see [getHeightInch()](../../com.aspose.cells/shape\#getHeightInch--) |
| [setHeightPt(double value)](#setHeightPt-double-) | For the description of this property, please see [getHeightPt()](../../com.aspose.cells/shape\#getHeightPt--) |
| [setHeightScale(int value)](#setHeightScale-int-) | For the description of this property, please see [getHeightScale()](../../com.aspose.cells/shape\#getHeightScale--) |
| [setHidden(boolean value)](#setHidden-boolean-) | For the description of this property, please see [isHidden()](../../com.aspose.cells/shape\#isHidden--) |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | For the description of this property, please see [getHtmlText()](../../com.aspose.cells/shape\#getHtmlText--) |
| [setInputRange(String value)](#setInputRange-java.lang.String-) | For the description of this property, please see [getInputRange()](../../com.aspose.cells/shape\#getInputRange--) |
| [setInputRange(String formula, boolean isR1C1, boolean isLocal)](#setInputRange-java.lang.String-boolean-boolean-) | Sets the range used to fill the control. |
| [setLeft(int value)](#setLeft-int-) | For the description of this property, please see [getLeft()](../../com.aspose.cells/shape\#getLeft--) |
| [setLeftCM(double value)](#setLeftCM-double-) | For the description of this property, please see [getLeftCM()](../../com.aspose.cells/shape\#getLeftCM--) |
| [setLeftInChart(int value)](#setLeftInChart-int-) | For the description of this property, please see [getLeftInChart()](../../com.aspose.cells/shape\#getLeftInChart--) |
| [setLeftInShape(int value)](#setLeftInShape-int-) | For the description of this property, please see [getLeftInShape()](../../com.aspose.cells/shape\#getLeftInShape--) |
| [setLeftInch(double value)](#setLeftInch-double-) | For the description of this property, please see [getLeftInch()](../../com.aspose.cells/shape\#getLeftInch--) |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | For the description of this property, please see [getLeftToCorner()](../../com.aspose.cells/shape\#getLeftToCorner--) |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | For the description of this property, please see [getLinkedCell()](../../com.aspose.cells/shape\#getLinkedCell--) |
| [setLinkedCell(String formula, boolean isR1C1, boolean isLocal)](#setLinkedCell-java.lang.String-boolean-boolean-) | Sets the range linked to the control's value. |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) | For the description of this property, please see [isLockAspectRatio()](../../com.aspose.cells/shape\#isLockAspectRatio--) |
| [setLocked(boolean value)](#setLocked-boolean-) | For the description of this property, please see [isLocked()](../../com.aspose.cells/shape\#isLocked--) |
| [setLockedProperty(int type, boolean value)](#setLockedProperty-int-boolean-) | Set the locked property. |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | For the description of this property, please see [getLowerDeltaX()](../../com.aspose.cells/shape\#getLowerDeltaX--) |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | For the description of this property, please see [getLowerDeltaY()](../../com.aspose.cells/shape\#getLowerDeltaY--) |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | For the description of this property, please see [getLowerRightColumn()](../../com.aspose.cells/shape\#getLowerRightColumn--) |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | For the description of this property, please see [getLowerRightRow()](../../com.aspose.cells/shape\#getLowerRightRow--) |
| [setMacroName(String value)](#setMacroName-java.lang.String-) | For the description of this property, please see [getMacroName()](../../com.aspose.cells/shape\#getMacroName--) |
| [setName(String value)](#setName-java.lang.String-) | For the description of this property, please see [getName()](../../com.aspose.cells/shape\#getName--) |
| [setPlacement(int value)](#setPlacement-int-) | For the description of this property, please see [getPlacement()](../../com.aspose.cells/shape\#getPlacement--) |
| [setPositionX(int value)](#setPositionX-int-) | For the description of this property, please see [getPositionX()](../../com.aspose.cells/shape\#getPositionX--) |
| [setPositionY(int value)](#setPositionY-int-) | For the description of this property, please see [getPositionY()](../../com.aspose.cells/shape\#getPositionY--) |
| [setPrintable(boolean value)](#setPrintable-boolean-) | For the description of this property, please see [isPrintable()](../../com.aspose.cells/shape\#isPrintable--) |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | For the description of this property, please see [getRelativeToOriginalPictureSize()](../../com.aspose.cells/shape\#getRelativeToOriginalPictureSize--) |
| [setRight(int value)](#setRight-int-) | For the description of this property, please see [getRight()](../../com.aspose.cells/shape\#getRight--) |
| [setRotationAngle(double value)](#setRotationAngle-double-) | For the description of this property, please see [getRotationAngle()](../../com.aspose.cells/shape\#getRotationAngle--) |
| [setSoftEdges(double value)](#setSoftEdges-double-) | For the description of this property, please see [getSoftEdges()](../../com.aspose.cells/shape\#getSoftEdges--) |
| [setText(String value)](#setText-java.lang.String-) | For the description of this property, please see [getText()](../../com.aspose.cells/shape\#getText--) |
| [setTextDirection(int value)](#setTextDirection-int-) | For the description of this property, please see [getTextDirection()](../../com.aspose.cells/shape\#getTextDirection--) |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | For the description of this property, please see [getTextHorizontalAlignment()](../../com.aspose.cells/shape\#getTextHorizontalAlignment--) |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | For the description of this property, please see [getTextHorizontalOverflow()](../../com.aspose.cells/shape\#getTextHorizontalOverflow--) |
| [setTextOptions(TextOptions value)](#setTextOptions-com.aspose.cells.TextOptions-) | For the description of this property, please see [getTextOptions()](../../com.aspose.cells/shape\#getTextOptions--) |
| [setTextOrientationType(int value)](#setTextOrientationType-int-) | For the description of this property, please see [getTextOrientationType()](../../com.aspose.cells/shape\#getTextOrientationType--) |
| [setTextShapeType(int value)](#setTextShapeType-int-) | For the description of this property, please see [getTextShapeType()](../../com.aspose.cells/shape\#getTextShapeType--) |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | For the description of this property, please see [getTextVerticalAlignment()](../../com.aspose.cells/shape\#getTextVerticalAlignment--) |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | For the description of this property, please see [getTextVerticalOverflow()](../../com.aspose.cells/shape\#getTextVerticalOverflow--) |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | For the description of this property, please see [isTextWrapped()](../../com.aspose.cells/shape\#isTextWrapped--) |
| [setTitle(String value)](#setTitle-java.lang.String-) | For the description of this property, please see [getTitle()](../../com.aspose.cells/shape\#getTitle--) |
| [setTop(int value)](#setTop-int-) | For the description of this property, please see [getTop()](../../com.aspose.cells/shape\#getTop--) |
| [setTopCM(double value)](#setTopCM-double-) | For the description of this property, please see [getTopCM()](../../com.aspose.cells/shape\#getTopCM--) |
| [setTopInChart(int value)](#setTopInChart-int-) | For the description of this property, please see [getTopInChart()](../../com.aspose.cells/shape\#getTopInChart--) |
| [setTopInShape(int value)](#setTopInShape-int-) | For the description of this property, please see [getTopInShape()](../../com.aspose.cells/shape\#getTopInShape--) |
| [setTopInch(double value)](#setTopInch-double-) | For the description of this property, please see [getTopInch()](../../com.aspose.cells/shape\#getTopInch--) |
| [setTopToCorner(int value)](#setTopToCorner-int-) | For the description of this property, please see [getTopToCorner()](../../com.aspose.cells/shape\#getTopToCorner--) |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | For the description of this property, please see [getUpperDeltaX()](../../com.aspose.cells/shape\#getUpperDeltaX--) |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | For the description of this property, please see [getUpperDeltaY()](../../com.aspose.cells/shape\#getUpperDeltaY--) |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | For the description of this property, please see [getUpperLeftColumn()](../../com.aspose.cells/shape\#getUpperLeftColumn--) |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | For the description of this property, please see [getUpperLeftRow()](../../com.aspose.cells/shape\#getUpperLeftRow--) |
| [setWidth(int value)](#setWidth-int-) | For the description of this property, please see [getWidth()](../../com.aspose.cells/shape\#getWidth--) |
| [setWidthCM(double value)](#setWidthCM-double-) | For the description of this property, please see [getWidthCM()](../../com.aspose.cells/shape\#getWidthCM--) |
| [setWidthInChart(int value)](#setWidthInChart-int-) | For the description of this property, please see [getWidthInChart()](../../com.aspose.cells/shape\#getWidthInChart--) |
| [setWidthInShape(int value)](#setWidthInShape-int-) | For the description of this property, please see [getWidthInShape()](../../com.aspose.cells/shape\#getWidthInShape--) |
| [setWidthInch(double value)](#setWidthInch-double-) | For the description of this property, please see [getWidthInch()](../../com.aspose.cells/shape\#getWidthInch--) |
| [setWidthPt(double value)](#setWidthPt-double-) | For the description of this property, please see [getWidthPt()](../../com.aspose.cells/shape\#getWidthPt--) |
| [setWidthScale(int value)](#setWidthScale-int-) | For the description of this property, please see [getWidthScale()](../../com.aspose.cells/shape\#getWidthScale--) |
| [setX(int value)](#setX-int-) | For the description of this property, please see [getX()](../../com.aspose.cells/shape\#getX--) |
| [setY(int value)](#setY-int-) | For the description of this property, please see [getY()](../../com.aspose.cells/shape\#getY--) |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | For the description of this property, please see [getZOrderPosition()](../../com.aspose.cells/shape\#getZOrderPosition--) |
| [toFrontOrBack(int orders)](#toFrontOrBack-int-) | Brings the shape to the front or sends the shape to back. |
| [toImage(OutputStream stream, ImageFormat imageFormat)](#toImage-java.io.OutputStream-com.aspose.cells.ImageFormat-) | Creates the shape image and saves it to a stream in the specified format. |
| [toImage(OutputStream stream, ImageOrPrintOptions options)](#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-) | Saves the shape to a stream. |
| [toImage(String imageFile, ImageOrPrintOptions options)](#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-) | Saves the shape to a file. |
| [toString()](#toString--) |  |
| [updateSelectedValue()](#updateSelectedValue--) | Update the selected value by the value of the linked cell. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String address) {#addHyperlink-java.lang.String-}
```
public Hyperlink addHyperlink(String address)
```


Adds a hyperlink to the shape.

```
Hyperlink hyperlink = shape.addHyperlink("https://www.aspose.com/");
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| address | java.lang.String | Address of the hyperlink. |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - Return the new hyperlink object.
### alignTopRightCorner(int topRow, int rightColumn) {#alignTopRightCorner-int-int-}
```
public void alignTopRightCorner(int topRow, int rightColumn)
```


Moves the picture to the top-right corner.

```
shape.alignTopRightCorner(2, 5);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | the row index. |
| rightColumn | int | the column index. |

### calculateTextSize() {#calculateTextSize--}
```
public int[] calculateTextSize()
```


Recalculate the text area

```
//The size of the text area is:w=size[0],h=size[1]
         int[] size = shape.calculateTextSize();
```

**Returns:**
int[] - Text's Size in an array(width and height).
### characters(int startIndex, int length) {#characters-int-int-}
```
public FontSetting characters(int startIndex, int length)
```


Returns a Characters object that represents a range of characters within the text. This method only works on shape with title.

```
FontSetting fontSetting = shape.characters(0, 4);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The index of the start of the character. |
| length | int | The number of characters. |

**Returns:**
[FontSetting](../../com.aspose.cells/fontsetting) - Characters object.
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### formatCharacters(int startIndex, int length, Font font) {#formatCharacters-int-int-com.aspose.cells.Font-}
```
public void formatCharacters(int startIndex, int length, Font font)
```


Formats some characters with the font setting. NOTE: This member is now obsolete. Instead, please use Shape.FormatCharacters(int startIndex, int length, Font font, StyleFlag flag) method. This property will be removed 12 months later since March 2016. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The start index. |
| length | int | The length. |
| font | [Font](../../com.aspose.cells/font) | The font setting. |

### formatCharacters(int startIndex, int length, Font font, StyleFlag flag) {#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-}
```
public void formatCharacters(int startIndex, int length, Font font, StyleFlag flag)
```


Formats some characters with the font setting.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startIndex | int | The start index. |
| length | int | The length. |
| font | [Font](../../com.aspose.cells/font) | The font setting. |
| flag | [StyleFlag](../../com.aspose.cells/styleflag) | The flag of the font setting. |

### getActiveXControl() {#getActiveXControl--}
```
public ActiveXControl getActiveXControl()
```


Gets the ActiveX control.

```
CheckBoxActiveXControl checkBox1 = (CheckBoxActiveXControl)shape.getActiveXControl();
         //The font name of CheckBox
         String fontName = checkBox1.getFont().getName();
```

**Returns:**
[ActiveXControl](../../com.aspose.cells/activexcontrol)
### getActualLowerRightRow() {#getActualLowerRightRow--}
```
public int getActualLowerRightRow()
```


Get the actual bottom row.

```
int rRow = shape.getActualLowerRightRow();
```

**Returns:**
int
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```


Returns or sets the descriptive (alternative) text string of the [Shape](../../com.aspose.cells/shape) object.

```
shape.setAlternativeText("a rectangle");
```

**Returns:**
java.lang.String
### getAnchorType() {#getAnchorType--}
```
public int getAnchorType()
```


the shape anchor placeholder.

```
if (shape.getAnchorType() == ShapeAnchorType.ONE_CELL_ANCHOR)
             shape.setAnchorType(ShapeAnchorType.TWO_CELL_ANCHOR);
```

**Returns:**
int
### getAutoShapeType() {#getAutoShapeType--}
```
public int getAutoShapeType()
```


the auto shape type.

```
if (shape.getAutoShapeType() == com.aspose.cells.AutoShapeType.UNKNOWN)
             shape.setAutoShapeType(com.aspose.cells.AutoShapeType.RECTANGLE);
```

**Returns:**
int
### getBottom() {#getBottom--}
```
public int getBottom()
```


Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels.

```
if (shape.getBottom() == 3)
             shape.setBottom(1);
```

**Returns:**
int
### getCharacters() {#getCharacters--}
```
public ArrayList getCharacters()
```


Returns all Characters objects that represents a range of characters within the text .

```
ArrayList list = shape.getCharacters();
```

**Returns:**
java.util.ArrayList - All Characters objects
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getComment() {#getComment--}
```
public Comment getComment()
```


Gets the comment object.

```
Comment comment = commentShape.getComment();
```

**Returns:**
[Comment](../../com.aspose.cells/comment)
### getConnectionPoints() {#getConnectionPoints--}
```
public float[][] getConnectionPoints()
```


Get the connection points

```
float[][] points = shape.getConnectionPoints();
```

**Returns:**
float[][] - [X,Y] pairs of the connection point. Every item is a float[2] array, [0] represents x and [1] represents y.
### getControlData() {#getControlData--}
```
public byte[] getControlData()
```


Gets the data of control.

```
if(shape.getControlData() == null)
             System.out.println("No data.");
```

**Returns:**
byte[]
### getCreateId() {#getCreateId--}
```
public UUID getCreateId()
```


create id for this shape.

**Returns:**
java.util.UUID
### getFill() {#getFill--}
```
public FillFormat getFill()
```


Returns a [Area.getFillFormat()](../../com.aspose.cells/area\#getFillFormat--) object that contains fill formatting properties for the specified shape.

```
FillFormat fillFmt = shape.getFill();
```

**Returns:**
[FillFormat](../../com.aspose.cells/fillformat)
### getFillFormat() {#getFillFormat--}
```
public MsoFillFormat getFillFormat()
```


Returns a MsoFillFormat object that contains fill formatting properties for the specified shape. NOTE: This member is now obsolete. Instead, please use Shape.Fill property. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
[MsoFillFormat](../../com.aspose.cells/msofillformat)
### getFont() {#getFont--}
```
public Font getFont()
```


Represents the font of shape.

```
Font font = shape.getFont();
         font.setName("Arial");
         font.setSize(12);
         font.setColor(Color.getRed());
```

**Returns:**
[Font](../../com.aspose.cells/font)
### getFormat() {#getFormat--}
```
public ShapeFormat getFormat()
```


Represents the setting of the shape's formatting. NOTE: This member is now obsolete. Instead, please use Shape.Fill and Shape.Line properties. This property will be removed 6 months later since August 2016. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
[ShapeFormat](../../com.aspose.cells/shapeformat)
### getFormatPicture() {#getFormatPicture--}
```
public MsoFormatPicture getFormatPicture()
```


the options of the picture format.

```
MsoFormatPicture msoFormatPicture = shape.getFormatPicture();
```

**Returns:**
[MsoFormatPicture](../../com.aspose.cells/msoformatpicture)
### getGeometry() {#getGeometry--}
```
public Geometry getGeometry()
```


Gets the geometry

```
if (shape.getGeometry().getShapeAdjustValues().getCount() == 0)
             System.out.println("No geometry path.");
```

**Returns:**
[Geometry](../../com.aspose.cells/geometry)
### getGlow() {#getGlow--}
```
public GlowEffect getGlow()
```


Represents a [ShapeFormat.getGlowEffect()](../../com.aspose.cells/shapeformat\#getGlowEffect--) object that specifies glow effect for the chart element or shape.

```
GlowEffect glowEffect = shape.getGlow();
```

**Returns:**
[GlowEffect](../../com.aspose.cells/gloweffect)
### getGroup() {#getGroup--}
```
public GroupShape getGroup()
```


Gets the group shape which contains this shape.

```
GroupShape groupShape = shape.getGroup();
```

**Returns:**
[GroupShape](../../com.aspose.cells/groupshape)
### getHeight() {#getHeight--}
```
public int getHeight()
```


Represents the height of shape, in unit of pixel.

```
if (shape.getHeight() == 3)
             shape.setHeight(1);
```

**Returns:**
int
### getHeightCM() {#getHeightCM--}
```
public double getHeightCM()
```


Represents the height of the shape, in unit of centimeters.

```
if (shape.getHeightCM() == 3)
             shape.setHeightCM(1);
```

**Returns:**
double
### getHeightInChart() {#getHeightInChart--}
```
public int getHeightInChart()
```


Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Drawing.Shape.HeightInShape property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getHeightInShape() {#getHeightInShape--}
```
public int getHeightInShape()
```


Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. Only Applies when this shape in the group or chart.

```
if (shape.getUpperDeltaY() == 4000)
             shape.setUpperDeltaY(2000);
```

**Returns:**
int
### getHeightInch() {#getHeightInch--}
```
public double getHeightInch()
```


Represents the height of the shape, in unit of inches.

```
if (shape.getHeightInch() == 3)
             shape.setHeightInch(1);
```

**Returns:**
double
### getHeightPt() {#getHeightPt--}
```
public double getHeightPt()
```


Represents the height of the shape, in unit of points.

```
if (shape.getHeightPt() == 3)
             shape.setHeightPt(1);
```

**Returns:**
double
### getHeightScale() {#getHeightScale--}
```
public int getHeightScale()
```


the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100;

```
if (shape.getHeightScale() == 3)
             shape.setHeightScale(1);
```

**Returns:**
int
### getHtmlText() {#getHtmlText--}
```
public String getHtmlText()
```


the html string which contains data and some formats in this textbox.

```
String html = shape.getHtmlText();
         if(html == null || "".equals(html))
         {
             shape.setHtmlText("<Font Style='FONT-FAMILY: Calibri;FONT-SIZE: 11pt;COLOR: #0000ff;TEXT-ALIGN: left;'>This is a <b>test</b>.</Font>");
         }
```

**Returns:**
java.lang.String
### getHyperlink() {#getHyperlink--}
```
public Hyperlink getHyperlink()
```


Gets the hyperlink of the shape.

```
Hyperlink hyperlink = shape.getHyperlink();
```

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink)
### getId() {#getId--}
```
public int getId()
```


Gets the identifier of this shape.

```
int id = shape.getId();
```

**Returns:**
int
### getInputRange() {#getInputRange--}
```
public String getInputRange()
```


the worksheet range used to fill the specified combo box.

```
if (shape.getInputRange().equals("$B$6:$B10"))
             shape.setInputRange("$A$1:$A$5");
```

**Returns:**
java.lang.String
### getInputRange(boolean isR1C1, boolean isLocal) {#getInputRange-boolean-boolean-}
```
public String getInputRange(boolean isR1C1, boolean isLocal)
```


Gets the range used to fill the control.

```
String range = shape.getInputRange(false, true);
         //If successful, a value like "$A$1:$A$3" will be returned
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns:**
java.lang.String - The range used to fill the control.
### getLeft() {#getLeft--}
```
public int getLeft()
```


Represents the horizontal offset of shape from its left column, in unit of pixels.

```
if (shape.getLeft() == 3)
             shape.setLeft(1);
```

**Returns:**
int
### getLeftCM() {#getLeftCM--}
```
public double getLeftCM()
```


Represents the horizontal offset of shape from its left column, in unit of centimeters.

```
if (shape.getLeftCM() == 3)
             shape.setLeftCM(1);
```

**Returns:**
double
### getLeftInChart() {#getLeftInChart--}
```
public int getLeftInChart()
```


Represents the vertical offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Drawing.Shape.LeftInShape property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getLeftInShape() {#getLeftInShape--}
```
public int getLeftInShape()
```


Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. Only Applies when this shape in the group or chart.

```
if (shape.getUpperDeltaY() == 2000)
             shape.setUpperDeltaY(4000);
```

**Returns:**
int
### getLeftInch() {#getLeftInch--}
```
public double getLeftInch()
```


Represents the horizontal offset of shape from its left column, in unit of inches.

```
if (shape.getLeftInch() == 3)
             shape.setLeftInch(1);
```

**Returns:**
double
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```


the horizonal offset of shape from worksheet left border.

```
if (shape.getLeftToCorner() == 3)
             shape.setLeftToCorner(1);
```

**Returns:**
int
### getLine() {#getLine--}
```
public LineFormat getLine()
```


Gets line style

```
LineFormat lineFmt = shape.getLine();
```

**Returns:**
[LineFormat](../../com.aspose.cells/lineformat)
### getLineFormat() {#getLineFormat--}
```
public MsoLineFormat getLineFormat()
```


Returns a MsoLineFormat object that contains line formatting properties for the specified shape. NOTE: This member is now obsolete. Instead, please use Shape.Line property. This property will be removed 12 months later since July 2016. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
[MsoLineFormat](../../com.aspose.cells/msolineformat)
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


the worksheet range linked to the control's value.

```
if (shape.getLinkedCell().equals("$B$6"))
             shape.setLinkedCell("A1");
```

**Returns:**
java.lang.String
### getLinkedCell(boolean isR1C1, boolean isLocal) {#getLinkedCell-boolean-boolean-}
```
public String getLinkedCell(boolean isR1C1, boolean isLocal)
```


Gets the range linked to the control's value.

```
//You may get results like '$A$1'
         String link = shape.getLinkedCell(false, false);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

**Returns:**
java.lang.String - The range linked to the control's value.
### getLockedProperty(int type) {#getLockedProperty-int-}
```
public boolean getLockedProperty(int type)
```


Gets the value of locked property.

```
int noAdjustHandles = 0;
         if (shape.getLockedProperty(ShapeLockType.ADJUST_HANDLES))
             noAdjustHandles = 1;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | The type of the shape locked property. |

**Returns:**
boolean - Returns the value of locked property.
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```


the shape's horizontal offset from its lower right corner column. The range of value is 0 to 1024.

```
if (shape.getLowerDeltaX() == 3)
             shape.setLowerDeltaX(1);
```

**Returns:**
int
### getLowerDeltaY() {#getLowerDeltaY--}
```
public int getLowerDeltaY()
```


the shape's vertical offset from its lower right corner row. The range of value is 0 to 256.

```
if (shape.getLowerDeltaY() == 3)
             shape.setLowerDeltaY(1);
```

**Returns:**
int
### getLowerRightColumn() {#getLowerRightColumn--}
```
public int getLowerRightColumn()
```


Represents lower right corner column index.

```
if (shape.getLowerRightColumn() == 3)
             shape.setLowerRightColumn(1);
```

**Returns:**
int
### getLowerRightRow() {#getLowerRightRow--}
```
public int getLowerRightRow()
```


Represents lower right corner row index.

```
if (shape.getLowerRightRow() == 3)
             shape.setLowerRightRow(1);
```

**Returns:**
int
### getMacroName() {#getMacroName--}
```
public String getMacroName()
```


the name of macro.

```
//Sets the name of macro.
         shape.setMacroName("DoWork()");
```

**Returns:**
java.lang.String
### getMsoDrawingType() {#getMsoDrawingType--}
```
public int getMsoDrawingType()
```


Gets mso drawing type.

```
/*Aspose.Cells.Drawing.MsoDrawingType*/int msoDrawingType = shape.getMsoDrawingType();
```

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


the name of the shape.

```
shape.setName("shape1");
```

**Returns:**
java.lang.String
### getPaths() {#getPaths--}
```
public ShapePathCollection getPaths()
```


Gets the paths of a custom geometric shape.

```
//Returns non-null if there is a path to the custom geometry
         if(shape.getPaths() == null)
             System.out.println("No custom geometry path.");
```

**Returns:**
[ShapePathCollection](../../com.aspose.cells/shapepathcollection)
### getPlacement() {#getPlacement--}
```
public int getPlacement()
```


Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet.

```
if (shape.getPlacement() == PlacementType.MOVE)
             shape.setPlacement(PlacementType.MOVE_AND_SIZE);
```

**Returns:**
int
### getPositionX() {#getPositionX--}
```
public int getPositionX()
```


the horizonal offset of shape from worksheet left border,in unit of pixels. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Drawing.Shape.X property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getPositionY() {#getPositionY--}
```
public int getPositionY()
```


the vertical offset of shape from worksheet top border,in unit of pixels. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Drawing.Shape.Y property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getReflection() {#getReflection--}
```
public ReflectionEffect getReflection()
```


Represents a [ReflectionEffect](../../com.aspose.cells/reflectioneffect) object that specifies reflection effect for the chart element or shape.

```
ReflectionEffect reflectionEffect = shape.getReflection();
```

**Returns:**
[ReflectionEffect](../../com.aspose.cells/reflectioneffect)
### getRelativeToOriginalPictureSize() {#getRelativeToOriginalPictureSize--}
```
public boolean getRelativeToOriginalPictureSize()
```


Indicates whether shape is relative to original picture size.

```
if(shape.getRelativeToOriginalPictureSize())
             shape.setRelativeToOriginalPictureSize(false);
```

**Returns:**
boolean
### getResultOfSmartArt() {#getResultOfSmartArt--}
```
public GroupShape getResultOfSmartArt()
```


Converting smart art to grouped shapes.

```
GroupShape groupShape = shape.getResultOfSmartArt();
```

**Returns:**
[GroupShape](../../com.aspose.cells/groupshape)
### getRight() {#getRight--}
```
public int getRight()
```


Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels.

```
if (shape.getRight() == 3)
             shape.setRight(1);
```

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


the rotation of the shape.

```
if(shape.getRotationAngle() == 45)
             shape.setRotationAngle(60);
```

**Returns:**
double
### getShadowEffect() {#getShadowEffect--}
```
public ShadowEffect getShadowEffect()
```


Represents a [ShadowEffect](../../com.aspose.cells/shadoweffect) object that specifies shadow effect for the chart element or shape.

```
ShadowEffect shadowEffect = shape.getShadowEffect();
```

**Returns:**
[ShadowEffect](../../com.aspose.cells/shadoweffect)
### getSoftEdges() {#getSoftEdges--}
```
public double getSoftEdges()
```


the radius of blur to apply to the edges, in unit of points.

```
shape.setSoftEdges(0.5d);
```

**Returns:**
double
### getSpid() {#getSpid--}
```
public String getSpid()
```


Specifies an optional string that an application can use to Identify the particular shape.

```
String spid = shape.getSpid();
```

**Returns:**
java.lang.String
### getSpt() {#getSpt--}
```
public int getSpt()
```


Specifies an optional number that an application can use to associate the particular shape with a defined shape type.

```
int spt = shape.getSpt();
```

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


Represents the string in this TextBox object.

```
if(shape.getText() == null)
             shape.setText("This is a test.");
```

**Returns:**
java.lang.String
### getTextBody() {#getTextBody--}
```
public FontSettingCollection getTextBody()
```


the setting of the shape's text.

```
FontSettingCollection fontSettingCollection = shape.getTextBody();
         fontSettingCollection.setText("This is a test.");
```

**Returns:**
[FontSettingCollection](../../com.aspose.cells/fontsettingcollection)
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Gets/Sets the direction of the text flow for this object.

```
if (shape.getTextDirection() == com.aspose.cells.TextDirectionType.CONTEXT)
             shape.setTextDirection(com.aspose.cells.TextDirectionType.LEFT_TO_RIGHT);
```

**Returns:**
int
### getTextEffect() {#getTextEffect--}
```
public TextEffectFormat getTextEffect()
```


Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape. Applies to Shape objects that represent WordArt.

```
TextEffectFormat textEffectFormat = shape.getTextEffect();
```

**Returns:**
[TextEffectFormat](../../com.aspose.cells/texteffectformat)
### getTextFrame() {#getTextFrame--}
```
public MsoTextFrame getTextFrame()
```


Returns a TextFrame object that contains the alignment and anchoring properties for the specified shape. NOTE: This member is now obsolete. Instead, please use Shape.TextBody.TextAlignment property. This property will be removed 12 months later since May 2016. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
[MsoTextFrame](../../com.aspose.cells/msotextframe)
### getTextHorizontalAlignment() {#getTextHorizontalAlignment--}
```
public int getTextHorizontalAlignment()
```


the text horizontal alignment type of the shape.

```
if (shape.getTextHorizontalAlignment() == com.aspose.cells.TextAlignmentType.BOTTOM)
             shape.setTextHorizontalAlignment(com.aspose.cells.TextAlignmentType.CENTER);
```

**Returns:**
int
### getTextHorizontalOverflow() {#getTextHorizontalOverflow--}
```
public int getTextHorizontalOverflow()
```


the text horizontal overflow type of the shape which contains text.

```
if (shape.getTextHorizontalOverflow() == com.aspose.cells.TextOverflowType.CLIP)
             shape.setTextHorizontalOverflow(com.aspose.cells.TextOverflowType.OVERFLOW);
```

**Returns:**
int
### getTextOptions() {#getTextOptions--}
```
public TextOptions getTextOptions()
```


Represents the text options of the shape.

```
TextOptions opt = shape.getTextOptions();
         opt.setColor(Color.getBlue());
         opt.setSize(8);
```

**Returns:**
[TextOptions](../../com.aspose.cells/textoptions)
### getTextOrientationType() {#getTextOrientationType--}
```
public int getTextOrientationType()
```


the text orientation type of the shape.

```
if (shape.getTextOrientationType() == com.aspose.cells.TextOrientationType.NO_ROTATION)
             shape.setTextOrientationType(com.aspose.cells.TextOrientationType.TOP_TO_BOTTOM);
```

**Returns:**
int
### getTextShapeType() {#getTextShapeType--}
```
public int getTextShapeType()
```


the preset text shape type.

```
if (shape.getTextShapeType() == com.aspose.cells.AutoShapeType.UNKNOWN)
             shape.setTextShapeType(com.aspose.cells.AutoShapeType.RECTANGLE);
```

**Returns:**
int
### getTextVerticalAlignment() {#getTextVerticalAlignment--}
```
public int getTextVerticalAlignment()
```


the text vertical alignment type of the shape.

```
if (shape.getTextVerticalAlignment() == com.aspose.cells.TextAlignmentType.BOTTOM)
             shape.setTextVerticalAlignment(com.aspose.cells.TextAlignmentType.CENTER);
```

**Returns:**
int
### getTextVerticalOverflow() {#getTextVerticalOverflow--}
```
public int getTextVerticalOverflow()
```


the text vertical overflow type of the shape which contains text.

```
if (shape.getTextVerticalOverflow() == com.aspose.cells.TextOverflowType.CLIP)
             shape.setTextVerticalOverflow(com.aspose.cells.TextOverflowType.OVERFLOW);
```

**Returns:**
int
### getThreeDFormat() {#getThreeDFormat--}
```
public ThreeDFormat getThreeDFormat()
```


3d format of the shape.

```
ThreeDFormat threeDFormat = shape.getThreeDFormat();
```

**Returns:**
[ThreeDFormat](../../com.aspose.cells/threedformat)
### getTitle() {#getTitle--}
```
public String getTitle()
```


Specifies the title (caption) of the current shape object.

```
shape.setTitle("title1");
```

**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


Represents the vertical offset of shape from its top row, in unit of pixels. If the shape is in the chart, represents the vertical offset of shape from its top border.

```
if (shape.getTop() == 3)
             shape.setTop(1);
```

**Returns:**
int
### getTopCM() {#getTopCM--}
```
public double getTopCM()
```


Represents the vertical offset of shape from its top row, in unit of centimeters.

```
if (shape.getTopCM() == 3)
             shape.setTopCM(1);
```

**Returns:**
double
### getTopInChart() {#getTopInChart--}
```
public int getTopInChart()
```


Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Drawing.Shape.TopInShape property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getTopInShape() {#getTopInShape--}
```
public int getTopInShape()
```


Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. Only Applies when this shape in the group or chart.

```
if (shape.getTopInShape() == 8000)
             shape.setTopInShape(4000);
```

**Returns:**
int
### getTopInch() {#getTopInch--}
```
public double getTopInch()
```


Represents the vertical offset of shape from its top row, in unit of inches.

```
if (shape.getTopInch() == 3)
             shape.setTopInch(1);
```

**Returns:**
double
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```


the vertical offset of shape from worksheet top border, in unit of pixels.

```
if (shape.getTopToCorner() == 3)
             shape.setTopToCorner(1);
```

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Gets the auto shape type.

```
/*Aspose.Cells.Drawing.AutoShapeType*/int autoShapeType = shape.getType();
```

**Returns:**
int
### getUpperDeltaX() {#getUpperDeltaX--}
```
public int getUpperDeltaX()
```


the shape's horizontal offset from its upper left corner column. The range of value is 0 to 1024.

```
if (shape.getUpperDeltaX() == 3)
             shape.setUpperDeltaX(1);
```

**Returns:**
int
### getUpperDeltaY() {#getUpperDeltaY--}
```
public int getUpperDeltaY()
```


the shape's vertical offset from its upper left corner row. The range of value is 0 to 256.

```
if (shape.getUpperDeltaY() == 3)
             shape.setUpperDeltaY(1);
```

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


Represents upper left corner column index.

```
if (shape.getUpperLeftColumn() == 3)
             shape.setUpperLeftColumn(1);
```

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


Represents upper left corner row index. If the shape is in the shape or in the group , UpperLeftRow will be ignored.

```
if (shape.getUpperLeftRow() == 3)
             shape.setUpperLeftRow(1);
```

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Represents the width of shape, in unit of pixels.

```
if (shape.getWidth() == 3)
             shape.setWidth(1);
```

**Returns:**
int
### getWidthCM() {#getWidthCM--}
```
public double getWidthCM()
```


Represents the width of the shape, in unit of centimeters.

```
if (shape.getWidthCM() == 3)
             shape.setWidthCM(1);
```

**Returns:**
double
### getWidthInChart() {#getWidthInChart--}
```
public int getWidthInChart()
```


Represents the width of the shape, in unit of 1/4000 of the parent shape. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Drawing.Shape.WidthInShape property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getWidthInShape() {#getWidthInShape--}
```
public int getWidthInShape()
```


Represents the width of the shape, in unit of 1/4000 of the parent shape. Only Applies when this shape in the group or chart.

```
if (shape.getUpperDeltaY() == 2000)
             shape.setUpperDeltaY(4000);
```

**Returns:**
int
### getWidthInch() {#getWidthInch--}
```
public double getWidthInch()
```


Represents the width of the shape, in unit of inch.

```
if (shape.getWidthInch() == 3)
             shape.setWidthInch(1);
```

**Returns:**
double
### getWidthPt() {#getWidthPt--}
```
public double getWidthPt()
```


Represents the width of the shape, in unit of point.

```
if (shape.getWidthPt() == 3)
             shape.setWidthPt(1);
```

**Returns:**
double
### getWidthScale() {#getWidthScale--}
```
public int getWidthScale()
```


the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100;

```
if (shape.getWidthScale() == 3)
             shape.setWidthScale(1);
```

**Returns:**
int
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Gets the [Range.getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) object which contains this shape.

```
Worksheet worksheet = shape.getWorksheet();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### getX() {#getX--}
```
public int getX()
```


the horizontal offset of shape from worksheet left border,in unit of pixels.

```
if (shape.getX() == 3)
             shape.setX(1);
```

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


the vertical offset of shape from worksheet top border,in unit of pixels.

```
if (shape.getY() == 3)
             shape.setY(1);
```

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


Returns the position of a shape in the z-order.

```
shape.setZOrderPosition(3);
```

**Returns:**
int
### hasLine() {#hasLine--}
```
public boolean hasLine()
```


the line border of the shape is visible.

```
if(shape.hasLine() == false)
             shape.setHasLine(true);
```

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isEquation() {#isEquation--}
```
public boolean isEquation()
```


Indicates whether the shape only contains an equation.

```
//If true,the shape only contains an equation.
         if(shape.isEquation())
         {
             //The shape contains only an equation
         }
```

**Returns:**
boolean
### isFilled() {#isFilled--}
```
public boolean isFilled()
```


Indicates whether the fill format is visible.

```
if(shape.isFilled() == false)
             shape.setFilled(true);
```

**Returns:**
boolean
### isFlippedHorizontally() {#isFlippedHorizontally--}
```
public boolean isFlippedHorizontally()
```


whether shape is horizontally flipped .

```
if(shape.isFlippedHorizontally() == false)
             shape.setFlippedHorizontally(true);
```

**Returns:**
boolean
### isFlippedVertically() {#isFlippedVertically--}
```
public boolean isFlippedVertically()
```


whether shape is vertically flipped .

```
if(shape.isFlippedVertically() == false)
             shape.setFlippedVertically(true);
```

**Returns:**
boolean
### isGroup() {#isGroup--}
```
public boolean isGroup()
```


Indicates whether the shape is a group.

```
if(shape.isGroup())
         {
             //This shape is a group.
         }
```

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Indicates whether the object is visible.

```
shape.setHidden(false);
```

**Returns:**
boolean
### isInGroup() {#isInGroup--}
```
public boolean isInGroup()
```


Indicates whether the shape is grouped.

**Returns:**
boolean
### isLockAspectRatio() {#isLockAspectRatio--}
```
public boolean isLockAspectRatio()
```


True means that don't allow changes in aspect ratio.

```
shape.setLockAspectRatio(false);
```

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


True if the object is locked, False if the object can be modified when the sheet is protected.

```
if(shape.isLocked())
             shape.setLocked(false);
```

**Returns:**
boolean
### isPrintable() {#isPrintable--}
```
public boolean isPrintable()
```


True if the object is printable

```
if(shape.isPrintable())
             shape.setPrintable(false);
```

**Returns:**
boolean
### isRichText() {#isRichText--}
```
public boolean isRichText()
```


Whether or not the text is rich text.

```
if(shape.isRichText())
             System.out.println("The text is rich text.");
```

**Returns:**
boolean
### isSameSetting(Object obj) {#isSameSetting-java.lang.Object-}
```
public boolean isSameSetting(Object obj)
```


Returns whether the shape is same.

```
if (shape.isSameSetting(shape))
             System.out.println("Two objects the same.");
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
boolean - 
### isSmartArt() {#isSmartArt--}
```
public boolean isSmartArt()
```


Indicates whether the shape is smart art. Only for ooxml file.

```
//if true,the shape is smart art.
         if(shape.isSmartArt())
         {
             //The shape is SmartArt object.
         }
```

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


the text wrapped type of the shape which contains text.

```
if (shape.isTextWrapped())
             shape.setTextWrapped(!shape.isTextWrapped());
```

**Returns:**
boolean
### isWordArt() {#isWordArt--}
```
public boolean isWordArt()
```


Indicates whether this shape is a word art. Only for the Legacy Shape of xls file.

```
if(shape.isWordArt())
         {
             //This shape is a WordArt object.
         }
```

**Returns:**
boolean
### moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn) {#moveToRange-int-int-int-int-}
```
public void moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)
```


Moves the shape to a specified range.

```
shape.moveToRange(12, 3, 13, 5);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int | Upper left row index. |
| upperLeftColumn | int | Upper left column index. |
| lowerRightRow | int | Lower right row index |
| lowerRightColumn | int | Lower right column index |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeActiveXControl() {#removeActiveXControl--}
```
public void removeActiveXControl()
```


Remove activeX control.

```
shape.removeActiveXControl();
```

### removeHyperlink() {#removeHyperlink--}
```
public void removeHyperlink()
```


Remove the hyperlink of the shape.

```
shape.removeHyperlink();
```

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


For the description of this property, please see [getAlternativeText()](../../com.aspose.cells/shape\#getAlternativeText--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setAnchorType(int value) {#setAnchorType-int-}
```
public void setAnchorType(int value)
```


For the description of this property, please see [getAnchorType()](../../com.aspose.cells/shape\#getAnchorType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setAutoShapeType(int value) {#setAutoShapeType-int-}
```
public void setAutoShapeType(int value)
```


For the description of this property, please see [getAutoShapeType()](../../com.aspose.cells/shape\#getAutoShapeType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setBottom(int value) {#setBottom-int-}
```
public void setBottom(int value)
```


For the description of this property, please see [getBottom()](../../com.aspose.cells/shape\#getBottom--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCreateId(UUID value) {#setCreateId-java.util.UUID-}
```
public void setCreateId(UUID value)
```


For the description of this property, please see [getCreateId()](../../com.aspose.cells/shape\#getCreateId--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.UUID |  |

### setFilled(boolean value) {#setFilled-boolean-}
```
public void setFilled(boolean value)
```


For the description of this property, please see [isFilled()](../../com.aspose.cells/shape\#isFilled--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFlippedHorizontally(boolean value) {#setFlippedHorizontally-boolean-}
```
public void setFlippedHorizontally(boolean value)
```


For the description of this property, please see [isFlippedHorizontally()](../../com.aspose.cells/shape\#isFlippedHorizontally--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```


For the description of this property, please see [isFlippedVertically()](../../com.aspose.cells/shape\#isFlippedVertically--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFont(Font value) {#setFont-com.aspose.cells.Font-}
```
public void setFont(Font value)
```


For the description of this property, please see [getFont()](../../com.aspose.cells/shape\#getFont--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Font](../../com.aspose.cells/font) |  |

### setHasLine(boolean value) {#setHasLine-boolean-}
```
public void setHasLine(boolean value)
```


For the description of this property, please see [hasLine()](../../com.aspose.cells/shape\#hasLine--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


For the description of this property, please see [getHeight()](../../com.aspose.cells/shape\#getHeight--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


For the description of this property, please see [getHeightCM()](../../com.aspose.cells/shape\#getHeightCM--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setHeightInChart(int value) {#setHeightInChart-int-}
```
public void setHeightInChart(int value)
```


For the description of this property, please see [getHeightInChart()](../../com.aspose.cells/shape\#getHeightInChart--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHeightInShape(int value) {#setHeightInShape-int-}
```
public void setHeightInShape(int value)
```


For the description of this property, please see [getHeightInShape()](../../com.aspose.cells/shape\#getHeightInShape--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


For the description of this property, please see [getHeightInch()](../../com.aspose.cells/shape\#getHeightInch--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setHeightPt(double value) {#setHeightPt-double-}
```
public void setHeightPt(double value)
```


For the description of this property, please see [getHeightPt()](../../com.aspose.cells/shape\#getHeightPt--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setHeightScale(int value) {#setHeightScale-int-}
```
public void setHeightScale(int value)
```


For the description of this property, please see [getHeightScale()](../../com.aspose.cells/shape\#getHeightScale--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


For the description of this property, please see [isHidden()](../../com.aspose.cells/shape\#isHidden--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHtmlText(String value) {#setHtmlText-java.lang.String-}
```
public void setHtmlText(String value)
```


For the description of this property, please see [getHtmlText()](../../com.aspose.cells/shape\#getHtmlText--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setInputRange(String value) {#setInputRange-java.lang.String-}
```
public void setInputRange(String value)
```


For the description of this property, please see [getInputRange()](../../com.aspose.cells/shape\#getInputRange--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setInputRange(String formula, boolean isR1C1, boolean isLocal) {#setInputRange-java.lang.String-boolean-boolean-}
```
public void setInputRange(String formula, boolean isR1C1, boolean isLocal)
```


Sets the range used to fill the control.

```
//After executing the code below, a ListBox object is created in the generated file. When the selected option is clicked, the selected value is displayed in cell A12.
 
         //Initialize a new workbook.
         //Workbook book = new Workbook();
 
         for (int i = 0; i? ++i)
         {
             Cell cell = book.getWorksheets().get(0).getCells().get(i, 0);
             cell.setValue(i + 1);
         }
 
         //Create a ListBox object
 
         //ActiveX Controls
         //Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,2, 0, 2, 0, 130, 130);
 
         //Form Controls
         Shape listBox = book.getWorksheets().get(0).getShapes().addListBox(2, 0, 2, 0, 130, 130);
 
         //Sets the range used to fill the control.
         listBox.setInputRange("$A$1:$A$6", false, false);
 
         //Sets the range linked to the control's value.
         listBox.setLinkedCell("$A$12", false, true);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | The range used to fill the control. |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

### setLeft(int value) {#setLeft-int-}
```
public void setLeft(int value)
```


For the description of this property, please see [getLeft()](../../com.aspose.cells/shape\#getLeft--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLeftCM(double value) {#setLeftCM-double-}
```
public void setLeftCM(double value)
```


For the description of this property, please see [getLeftCM()](../../com.aspose.cells/shape\#getLeftCM--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setLeftInChart(int value) {#setLeftInChart-int-}
```
public void setLeftInChart(int value)
```


For the description of this property, please see [getLeftInChart()](../../com.aspose.cells/shape\#getLeftInChart--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLeftInShape(int value) {#setLeftInShape-int-}
```
public void setLeftInShape(int value)
```


For the description of this property, please see [getLeftInShape()](../../com.aspose.cells/shape\#getLeftInShape--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLeftInch(double value) {#setLeftInch-double-}
```
public void setLeftInch(double value)
```


For the description of this property, please see [getLeftInch()](../../com.aspose.cells/shape\#getLeftInch--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setLeftToCorner(int value) {#setLeftToCorner-int-}
```
public void setLeftToCorner(int value)
```


For the description of this property, please see [getLeftToCorner()](../../com.aspose.cells/shape\#getLeftToCorner--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


For the description of this property, please see [getLinkedCell()](../../com.aspose.cells/shape\#getLinkedCell--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setLinkedCell(String formula, boolean isR1C1, boolean isLocal) {#setLinkedCell-java.lang.String-boolean-boolean-}
```
public void setLinkedCell(String formula, boolean isR1C1, boolean isLocal)
```


Sets the range linked to the control's value.

```
//After executing the code below, a ScrollBar object is created in the generated file. As you drag the slider, the value is displayed in cell A12.
 
         //ActiveX Controls
         //Aspose.Cells.Drawing.Shape scrollBar = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ScrollBar,2, 0, 2, 0, 30, 130);
 
         //Form Controls
         Shape scrollBar = book.getWorksheets().get(0).getShapes().addScrollBar(2, 0, 2, 0, 130, 30);
 
         //Sets the range linked to the control's value.
         scrollBar.setLinkedCell("$A$12", false, true);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | The range linked to the control's value. |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |

### setLockAspectRatio(boolean value) {#setLockAspectRatio-boolean-}
```
public void setLockAspectRatio(boolean value)
```


For the description of this property, please see [isLockAspectRatio()](../../com.aspose.cells/shape\#isLockAspectRatio--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


For the description of this property, please see [isLocked()](../../com.aspose.cells/shape\#isLocked--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLockedProperty(int type, boolean value) {#setLockedProperty-int-boolean-}
```
public void setLockedProperty(int type, boolean value)
```


Set the locked property.

```
shape.setLockedProperty(ShapeLockType.ADJUST_HANDLES, true);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | The locked type. |
| value | boolean | The value of the property. |

### setLowerDeltaX(int value) {#setLowerDeltaX-int-}
```
public void setLowerDeltaX(int value)
```


For the description of this property, please see [getLowerDeltaX()](../../com.aspose.cells/shape\#getLowerDeltaX--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLowerDeltaY(int value) {#setLowerDeltaY-int-}
```
public void setLowerDeltaY(int value)
```


For the description of this property, please see [getLowerDeltaY()](../../com.aspose.cells/shape\#getLowerDeltaY--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLowerRightColumn(int value) {#setLowerRightColumn-int-}
```
public void setLowerRightColumn(int value)
```


For the description of this property, please see [getLowerRightColumn()](../../com.aspose.cells/shape\#getLowerRightColumn--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLowerRightRow(int value) {#setLowerRightRow-int-}
```
public void setLowerRightRow(int value)
```


For the description of this property, please see [getLowerRightRow()](../../com.aspose.cells/shape\#getLowerRightRow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMacroName(String value) {#setMacroName-java.lang.String-}
```
public void setMacroName(String value)
```


For the description of this property, please see [getMacroName()](../../com.aspose.cells/shape\#getMacroName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


For the description of this property, please see [getName()](../../com.aspose.cells/shape\#getName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


For the description of this property, please see [getPlacement()](../../com.aspose.cells/shape\#getPlacement--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPositionX(int value) {#setPositionX-int-}
```
public void setPositionX(int value)
```


For the description of this property, please see [getPositionX()](../../com.aspose.cells/shape\#getPositionX--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPositionY(int value) {#setPositionY-int-}
```
public void setPositionY(int value)
```


For the description of this property, please see [getPositionY()](../../com.aspose.cells/shape\#getPositionY--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPrintable(boolean value) {#setPrintable-boolean-}
```
public void setPrintable(boolean value)
```


For the description of this property, please see [isPrintable()](../../com.aspose.cells/shape\#isPrintable--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRelativeToOriginalPictureSize(boolean value) {#setRelativeToOriginalPictureSize-boolean-}
```
public void setRelativeToOriginalPictureSize(boolean value)
```


For the description of this property, please see [getRelativeToOriginalPictureSize()](../../com.aspose.cells/shape\#getRelativeToOriginalPictureSize--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRight(int value) {#setRight-int-}
```
public void setRight(int value)
```


For the description of this property, please see [getRight()](../../com.aspose.cells/shape\#getRight--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


For the description of this property, please see [getRotationAngle()](../../com.aspose.cells/shape\#getRotationAngle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setSoftEdges(double value) {#setSoftEdges-double-}
```
public void setSoftEdges(double value)
```


For the description of this property, please see [getSoftEdges()](../../com.aspose.cells/shape\#getSoftEdges--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


For the description of this property, please see [getText()](../../com.aspose.cells/shape\#getText--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


For the description of this property, please see [getTextDirection()](../../com.aspose.cells/shape\#getTextDirection--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


For the description of this property, please see [getTextHorizontalAlignment()](../../com.aspose.cells/shape\#getTextHorizontalAlignment--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```


For the description of this property, please see [getTextHorizontalOverflow()](../../com.aspose.cells/shape\#getTextHorizontalOverflow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextOptions(TextOptions value) {#setTextOptions-com.aspose.cells.TextOptions-}
```
public void setTextOptions(TextOptions value)
```


For the description of this property, please see [getTextOptions()](../../com.aspose.cells/shape\#getTextOptions--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextOptions](../../com.aspose.cells/textoptions) |  |

### setTextOrientationType(int value) {#setTextOrientationType-int-}
```
public void setTextOrientationType(int value)
```


For the description of this property, please see [getTextOrientationType()](../../com.aspose.cells/shape\#getTextOrientationType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```


For the description of this property, please see [getTextShapeType()](../../com.aspose.cells/shape\#getTextShapeType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


For the description of this property, please see [getTextVerticalAlignment()](../../com.aspose.cells/shape\#getTextVerticalAlignment--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```


For the description of this property, please see [getTextVerticalOverflow()](../../com.aspose.cells/shape\#getTextVerticalOverflow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


For the description of this property, please see [isTextWrapped()](../../com.aspose.cells/shape\#isTextWrapped--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


For the description of this property, please see [getTitle()](../../com.aspose.cells/shape\#getTitle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setTop(int value) {#setTop-int-}
```
public void setTop(int value)
```


For the description of this property, please see [getTop()](../../com.aspose.cells/shape\#getTop--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTopCM(double value) {#setTopCM-double-}
```
public void setTopCM(double value)
```


For the description of this property, please see [getTopCM()](../../com.aspose.cells/shape\#getTopCM--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setTopInChart(int value) {#setTopInChart-int-}
```
public void setTopInChart(int value)
```


For the description of this property, please see [getTopInChart()](../../com.aspose.cells/shape\#getTopInChart--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTopInShape(int value) {#setTopInShape-int-}
```
public void setTopInShape(int value)
```


For the description of this property, please see [getTopInShape()](../../com.aspose.cells/shape\#getTopInShape--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTopInch(double value) {#setTopInch-double-}
```
public void setTopInch(double value)
```


For the description of this property, please see [getTopInch()](../../com.aspose.cells/shape\#getTopInch--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setTopToCorner(int value) {#setTopToCorner-int-}
```
public void setTopToCorner(int value)
```


For the description of this property, please see [getTopToCorner()](../../com.aspose.cells/shape\#getTopToCorner--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setUpperDeltaX(int value) {#setUpperDeltaX-int-}
```
public void setUpperDeltaX(int value)
```


For the description of this property, please see [getUpperDeltaX()](../../com.aspose.cells/shape\#getUpperDeltaX--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setUpperDeltaY(int value) {#setUpperDeltaY-int-}
```
public void setUpperDeltaY(int value)
```


For the description of this property, please see [getUpperDeltaY()](../../com.aspose.cells/shape\#getUpperDeltaY--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setUpperLeftColumn(int value) {#setUpperLeftColumn-int-}
```
public void setUpperLeftColumn(int value)
```


For the description of this property, please see [getUpperLeftColumn()](../../com.aspose.cells/shape\#getUpperLeftColumn--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setUpperLeftRow(int value) {#setUpperLeftRow-int-}
```
public void setUpperLeftRow(int value)
```


For the description of this property, please see [getUpperLeftRow()](../../com.aspose.cells/shape\#getUpperLeftRow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


For the description of this property, please see [getWidth()](../../com.aspose.cells/shape\#getWidth--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


For the description of this property, please see [getWidthCM()](../../com.aspose.cells/shape\#getWidthCM--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWidthInChart(int value) {#setWidthInChart-int-}
```
public void setWidthInChart(int value)
```


For the description of this property, please see [getWidthInChart()](../../com.aspose.cells/shape\#getWidthInChart--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setWidthInShape(int value) {#setWidthInShape-int-}
```
public void setWidthInShape(int value)
```


For the description of this property, please see [getWidthInShape()](../../com.aspose.cells/shape\#getWidthInShape--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


For the description of this property, please see [getWidthInch()](../../com.aspose.cells/shape\#getWidthInch--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWidthPt(double value) {#setWidthPt-double-}
```
public void setWidthPt(double value)
```


For the description of this property, please see [getWidthPt()](../../com.aspose.cells/shape\#getWidthPt--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWidthScale(int value) {#setWidthScale-int-}
```
public void setWidthScale(int value)
```


For the description of this property, please see [getWidthScale()](../../com.aspose.cells/shape\#getWidthScale--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


For the description of this property, please see [getX()](../../com.aspose.cells/shape\#getX--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


For the description of this property, please see [getY()](../../com.aspose.cells/shape\#getY--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```


For the description of this property, please see [getZOrderPosition()](../../com.aspose.cells/shape\#getZOrderPosition--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### toFrontOrBack(int orders) {#toFrontOrBack-int-}
```
public void toFrontOrBack(int orders)
```


Brings the shape to the front or sends the shape to back.

```
shape.toFrontOrBack(2);
         //or shape.ToFrontOrBack(-1);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| orders | int | If it's less than zero, sets the shape to back. If it's greater than zero, brings the shape to front. |

### toImage(OutputStream stream, ImageFormat imageFormat) {#toImage-java.io.OutputStream-com.aspose.cells.ImageFormat-}
```
public void toImage(OutputStream stream, ImageFormat imageFormat)
```


Creates the shape image and saves it to a stream in the specified format.

The following formats are supported: .bmp, .gif, .jpg, .jpeg, .tiff, .emf.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream | The output stream. |
| imageFormat | [ImageFormat](../../com.aspose.cells/imageformat) | The format in which to save the image. |

### toImage(OutputStream stream, ImageOrPrintOptions options) {#toImage-java.io.OutputStream-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(OutputStream stream, ImageOrPrintOptions options)
```


Saves the shape to a stream.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stream | java.io.OutputStream |  |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

### toImage(String imageFile, ImageOrPrintOptions options) {#toImage-java.lang.String-com.aspose.cells.ImageOrPrintOptions-}
```
public void toImage(String imageFile, ImageOrPrintOptions options)
```


Saves the shape to a file.

```
ImageOrPrintOptions op = new ImageOrPrintOptions();
         shape.toImage("exmaple.png", op);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| imageFile | java.lang.String |  |
| options | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### updateSelectedValue() {#updateSelectedValue--}
```
public void updateSelectedValue()
```


Update the selected value by the value of the linked cell.

```
//Initialize a new workbook.
         //Workbook book = new Workbook();
 
         Cell cell = null;
         for (int i = 0; i? ++i)
         {
             cell = book.getWorksheets().get(0).getCells().get(i, 0);
             cell.setValue(i + 1);
         }
 
         //Create a ListBox object
 
         //ActiveX Controls
         //Aspose.Cells.Drawing.Shape listBox = book.Worksheets[0].Shapes.AddActiveXControl( Aspose.Cells.Drawing.ActiveXControls.ControlType.ListBox,2, 0, 2, 0, 130, 130);
 
         //Form Controls
         Shape listBox = book.getWorksheets().get(0).getShapes().addListBox(2, 0, 2, 0, 130, 130);
 
         //Sets the range used to fill the control.
         listBox.setInputRange("$A$1:$A$6", false, false);
 
         //Sets the range linked to the control's value.
         listBox.setLinkedCell("$A$12", false, true);
 
         ListBox listbx = (ListBox)listBox;
 
         //Set the value of cell A12
         cell = book.getWorksheets().get(0).getCells().get(11, 0);
         cell.setValue(3);
 
         //Update the selected value by the value of the linked cell.
         listBox.updateSelectedValue();
 
         //-1 default, no option selected
         if(listbx.isSelected(2))
         {
             //Option 3 of the ListBox is selected
         }
 
         //Change the value of a linked cell
         cell.setValue(4);
 
         //Update the selected value by the value of the linked cell.
         listBox.updateSelectedValue();
         if(listbx.isSelected(3))
         {
             //Option 4 of the ListBox is selected
         }
```

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

