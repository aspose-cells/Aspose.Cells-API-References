---
title: Picture
second_title: Aspose.Cells for Java API Reference
description: Encapsulates the object that represents a single picture in a spreadsheet.
type: docs
url: /java/com.aspose.cells/picture/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.Shape](../../com.aspose.cells/shape)
```
public class Picture extends Shape
```

Encapsulates the object that represents a single picture in a spreadsheet.

**Example**

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //Adding a new worksheet to the Workbook object
         int sheetIndex = workbook.getWorksheets().add();
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(sheetIndex);
         //Adding a picture at the location of a cell whose row and column indices
         //are 5 in the worksheet. It is "F6" cell
         worksheet.getPictures().add(5, 5, "image.gif");
         //Saving the Excel file
         workbook.save("book1.xls", SaveFormat.EXCEL_97_TO_2003);
```
## Methods

| Method | Description |
| --- | --- |
| [addHyperlink(String address)](#addHyperlink-java.lang.String-) | Adds a hyperlink to the shape. |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | Moves the picture to the top-right corner. |
| [calculateTextSize()](#calculateTextSize--) | Recalculate the text area |
| [characters(int startIndex, int length)](#characters-int-int-) | Returns a Characters object that represents a range of characters within the text. |
| [copy(Picture source, CopyOptions options)](#copy-com.aspose.cells.Picture-com.aspose.cells.CopyOptions-) | Copy the picture. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [formatCharacters(int startIndex, int length, Font font)](#formatCharacters-int-int-com.aspose.cells.Font-) | Formats some characters with the font setting. |
| [formatCharacters(int startIndex, int length, Font font, StyleFlag flag)](#formatCharacters-int-int-com.aspose.cells.Font-com.aspose.cells.StyleFlag-) | Formats some characters with the font setting. |
| [getActiveXControl()](#getActiveXControl--) | Gets the ActiveX control. |
| [getActualLowerRightRow()](#getActualLowerRightRow--) | Get the actual bottom row. |
| [getAlternativeText()](#getAlternativeText--) | Returns or sets the descriptive (alternative) text string of the [Shape](../../com.aspose.cells/shape) object. |
| [getAnchorType()](#getAnchorType--) | Gets the shape anchor placeholder. |
| [getAutoShapeType()](#getAutoShapeType--) | Gets the auto shape type. |
| [getBorderLineColor()](#getBorderLineColor--) | Represents the [Color](../../com.aspose.cells/color) of the border line of a picture. |
| [getBorderWeight()](#getBorderWeight--) | Gets the weight of the border line of a picture in units of pt. |
| [getBottom()](#getBottom--) | Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels. |
| [getCharacters()](#getCharacters--) | Returns all Characters objects that represents a range of characters within the text . |
| [getClass()](#getClass--) |  |
| [getConnectionPoints()](#getConnectionPoints--) | Get the connection points |
| [getControlData()](#getControlData--) | Gets the data of control. |
| [getCreateId()](#getCreateId--) | Gets create id for this shape. |
| [getData()](#getData--) | Gets the data of the picture. |
| [getDisplayAsIcon()](#getDisplayAsIcon--) | True if the specified object is displayed as an icon and the image will not be auto changed. |
| [getFill()](#getFill--) | Returns a [Area.getFillFormat()](../../com.aspose.cells/area\#getFillFormat--) object that contains fill formatting properties for the specified shape. |
| [getFillFormat()](#getFillFormat--) | Returns a MsoFillFormat object that contains fill formatting properties for the specified shape. |
| [getFont()](#getFont--) | Represents the font of shape. |
| [getFormatPicture()](#getFormatPicture--) | Gets the options of the picture format. |
| [getFormula()](#getFormula--) | Gets the data of the formula. |
| [getGeometry()](#getGeometry--) | Gets the geometry |
| [getGlow()](#getGlow--) | Represents a [ShapePropertyCollection.getGlowEffect()](../../com.aspose.cells/shapepropertycollection\#getGlowEffect--) object that specifies glow effect for the chart element or shape. |
| [getGroup()](#getGroup--) | Gets the group shape which contains this shape. |
| [getHeight()](#getHeight--) | Represents the height of shape, in unit of pixel. |
| [getHeightCM()](#getHeightCM--) | Represents the height of the shape, in unit of centimeters. |
| [getHeightInChart()](#getHeightInChart--) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. |
| [getHeightInShape()](#getHeightInShape--) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. |
| [getHeightInch()](#getHeightInch--) | Represents the height of the shape, in unit of inches. |
| [getHeightPt()](#getHeightPt--) | Represents the height of the shape, in unit of points. |
| [getHeightScale()](#getHeightScale--) | Gets the height scale,in unit of percent of the original picture height. |
| [getHtmlText()](#getHtmlText--) | Gets the html string which contains data and some formats in this textbox. |
| [getHyperlink()](#getHyperlink--) | Gets the hyperlink of the shape. |
| [getId()](#getId--) | Gets the identifier of this shape. |
| [getImageType()](#getImageType--) | Gets the image format of the picture. |
| [getInputRange()](#getInputRange--) | Gets the worksheet range used to fill the specified combo box. |
| [getInputRange(boolean isR1C1, boolean isLocal)](#getInputRange-boolean-boolean-) | Gets the range used to fill the control. |
| [getLeft()](#getLeft--) | Represents the horizontal offset of shape from its left column, in unit of pixels. |
| [getLeftCM()](#getLeftCM--) | Represents the horizontal offset of shape from its left column, in unit of centimeters. |
| [getLeftInChart()](#getLeftInChart--) | Represents the vertical offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. |
| [getLeftInShape()](#getLeftInShape--) | Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. |
| [getLeftInch()](#getLeftInch--) | Represents the horizontal offset of shape from its left column, in unit of inches. |
| [getLeftToCorner()](#getLeftToCorner--) | Gets the horizonal offset of shape from worksheet left border. |
| [getLine()](#getLine--) | Gets line style |
| [getLineFormat()](#getLineFormat--) | Returns a MsoLineFormat object that contains line formatting properties for the specified shape. |
| [getLinkedCell()](#getLinkedCell--) | Gets the worksheet range linked to the control's value. |
| [getLinkedCell(boolean isR1C1, boolean isLocal)](#getLinkedCell-boolean-boolean-) | Gets the range linked to the control's value. |
| [getLockedProperty(int type)](#getLockedProperty-int-) | Gets the value of locked property. |
| [getLowerDeltaX()](#getLowerDeltaX--) | Gets the shape's horizontal offset from its lower right corner column. |
| [getLowerDeltaY()](#getLowerDeltaY--) | Gets the shape's vertical offset from its lower right corner row. |
| [getLowerRightColumn()](#getLowerRightColumn--) | Represents lower right corner column index. |
| [getLowerRightRow()](#getLowerRightRow--) | Represents lower right corner row index. |
| [getMacroName()](#getMacroName--) | Gets the name of macro. |
| [getMsoDrawingType()](#getMsoDrawingType--) | Gets mso drawing type. |
| [getName()](#getName--) | Gets the name of the shape. |
| [getOriginalHeight()](#getOriginalHeight--) | Gets the original height of the picture. |
| [getOriginalHeightCM()](#getOriginalHeightCM--) | Gets the original height of picture, in unit of centimeters. |
| [getOriginalHeightInch()](#getOriginalHeightInch--) | Gets the original height of picture, in unit of inches. |
| [getOriginalWidth()](#getOriginalWidth--) | Gets the original width of the picture. |
| [getOriginalWidthCM()](#getOriginalWidthCM--) | Gets the original width of picture, in unit of centimeters. |
| [getOriginalWidthInch()](#getOriginalWidthInch--) | Gets the original width of picture, in unit of inches. |
| [getPaths()](#getPaths--) | Gets the paths of a custom geometric shape. |
| [getPlacement()](#getPlacement--) | Represents the way the drawing object is attached to the cells below it. |
| [getPositionX()](#getPositionX--) | Gets the horizonal offset of shape from worksheet left border,in unit of pixels. |
| [getPositionY()](#getPositionY--) | Gets the vertical offset of shape from worksheet top border,in unit of pixels. |
| [getReflection()](#getReflection--) | Represents a [ReflectionEffect](../../com.aspose.cells/reflectioneffect) object that specifies reflection effect for the chart element or shape. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | Indicates whether shape is relative to original picture size. |
| [getResultOfSmartArt()](#getResultOfSmartArt--) | Converting smart art to grouped shapes. |
| [getRight()](#getRight--) | Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels. |
| [getRotationAngle()](#getRotationAngle--) | Gets the rotation of the shape. |
| [getShadowEffect()](#getShadowEffect--) | Represents a [ShadowEffect](../../com.aspose.cells/shadoweffect) object that specifies shadow effect for the chart element or shape. |
| [getSignatureLine()](#getSignatureLine--) | Gets the signature line |
| [getSoftEdges()](#getSoftEdges--) | Gets the radius of blur to apply to the edges, in unit of points. |
| [getSourceFullName()](#getSourceFullName--) | Gets the path and name of the source file for the linked image. |
| [getSpid()](#getSpid--) | Specifies an optional string that an application can use to Identify the particular shape. |
| [getSpt()](#getSpt--) | Specifies an optional number that an application can use to associate the particular shape with a defined shape type. |
| [getText()](#getText--) | Represents the string in this TextBox object. |
| [getTextBody()](#getTextBody--) | Gets the setting of the shape's text. |
| [getTextDirection()](#getTextDirection--) | Gets the direction of the text flow for this object. |
| [getTextEffect()](#getTextEffect--) | Returns a TextEffectFormat object that contains text-effect formatting properties for the specified shape. |
| [getTextFrame()](#getTextFrame--) | Returns a TextFrame object that contains the alignment and anchoring properties for the specified shape. |
| [getTextHorizontalAlignment()](#getTextHorizontalAlignment--) | Gets the text horizontal alignment type of the shape. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | Gets the text horizontal overflow type of the shape which contains text. |
| [getTextOptions()](#getTextOptions--) | Represents the text options of the shape. |
| [getTextOrientationType()](#getTextOrientationType--) | Gets the text orientation type of the shape. |
| [getTextShapeType()](#getTextShapeType--) | Gets the preset text shape type. |
| [getTextVerticalAlignment()](#getTextVerticalAlignment--) | Gets the text vertical alignment type of the shape. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | Gets the text vertical overflow type of the shape which contains text. |
| [getThreeDFormat()](#getThreeDFormat--) | Gets 3d format of the shape. |
| [getTitle()](#getTitle--) | Specifies the title (caption) of the current shape object. |
| [getTop()](#getTop--) | Represents the vertical offset of shape from its top row, in unit of pixels. |
| [getTopCM()](#getTopCM--) | Represents the vertical offset of shape from its top row, in unit of centimeters. |
| [getTopInChart()](#getTopInChart--) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. |
| [getTopInShape()](#getTopInShape--) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. |
| [getTopInch()](#getTopInch--) | Represents the vertical offset of shape from its top row, in unit of inches. |
| [getTopToCorner()](#getTopToCorner--) | Gets the vertical offset of shape from worksheet top border, in unit of pixels. |
| [getType()](#getType--) | Gets the auto shape type. |
| [getUpperDeltaX()](#getUpperDeltaX--) | Gets the shape's horizontal offset from its upper left corner column. |
| [getUpperDeltaY()](#getUpperDeltaY--) | Gets the shape's vertical offset from its upper left corner row. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Represents upper left corner column index. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Represents upper left corner row index. |
| [getWidth()](#getWidth--) | Represents the width of shape, in unit of pixels. |
| [getWidthCM()](#getWidthCM--) | Represents the width of the shape, in unit of centimeters. |
| [getWidthInChart()](#getWidthInChart--) | Represents the width of the shape, in unit of 1/4000 of the parent shape. |
| [getWidthInShape()](#getWidthInShape--) | Represents the width of the shape, in unit of 1/4000 of the parent shape. |
| [getWidthInch()](#getWidthInch--) | Represents the width of the shape, in unit of inch. |
| [getWidthPt()](#getWidthPt--) | Represents the width of the shape, in unit of point. |
| [getWidthScale()](#getWidthScale--) | Gets the width scale, in unit of percent of the original picture width. |
| [getWorksheet()](#getWorksheet--) | Gets the [Range.getWorksheet()](../../com.aspose.cells/range\#getWorksheet--) object which contains this shape. |
| [getX()](#getX--) | Gets the horizontal offset of shape from worksheet left border,in unit of pixels. |
| [getY()](#getY--) | Gets the vertical offset of shape from worksheet top border,in unit of pixels. |
| [getZOrderPosition()](#getZOrderPosition--) | Returns the position of a shape in the z-order. |
| [hasLine()](#hasLine--) | Gets the line border of the shape is visible. |
| [hashCode()](#hashCode--) |  |
| [isAutoSize()](#isAutoSize--) | True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated. |
| [isDynamicDataExchange()](#isDynamicDataExchange--) | Gets whether dynamic data exchange |
| [isEquation()](#isEquation--) | Indicates whether the shape only contains an equation. |
| [isFilled()](#isFilled--) | Indicates whether the fill format is visible. |
| [isFlippedHorizontally()](#isFlippedHorizontally--) | Gets whether shape is horizontally flipped . |
| [isFlippedVertically()](#isFlippedVertically--) | Gets whether shape is vertically flipped . |
| [isGroup()](#isGroup--) | Indicates whether the shape is a group. |
| [isHidden()](#isHidden--) | Indicates whether the object is visible. |
| [isInGroup()](#isInGroup--) | Indicates whether the shape is grouped. |
| [isLink()](#isLink--) | Returns true if the picture is linked to a file. |
| [isLockAspectRatio()](#isLockAspectRatio--) | True means that don't allow changes in aspect ratio. |
| [isLocked()](#isLocked--) | True if the object is locked, False if the object can be modified when the sheet is protected. |
| [isPrintable()](#isPrintable--) | True if the object is printable |
| [isRichText()](#isRichText--) | Whether or not the text is rich text. |
| [isSameSetting(Object obj)](#isSameSetting-java.lang.Object-) | Returns whether the shape is same. |
| [isSmartArt()](#isSmartArt--) | Indicates whether the shape is smart art. |
| [isTextWrapped()](#isTextWrapped--) | Gets the text wrapped type of the shape which contains text. |
| [isWordArt()](#isWordArt--) | Indicates whether this shape is a word art. |
| [move(int upperLeftRow, int upperLeftColumn)](#move-int-int-) | Moves the picture to a specified location. |
| [moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)](#moveToRange-int-int-int-int-) | Moves the shape to a specified range. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeActiveXControl()](#removeActiveXControl--) | Remove activeX control. |
| [removeHyperlink()](#removeHyperlink--) | Remove the hyperlink of the shape. |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Returns or sets the descriptive (alternative) text string of the [Shape](../../com.aspose.cells/shape) object. |
| [setAnchorType(int value)](#setAnchorType-int-) | Sets the shape anchor placeholder. |
| [setAutoShapeType(int value)](#setAutoShapeType-int-) | Sets the auto shape type. |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated. |
| [setBorderLineColor(Color value)](#setBorderLineColor-com.aspose.cells.Color-) | Represents the [Color](../../com.aspose.cells/color) of the border line of a picture. |
| [setBorderWeight(double value)](#setBorderWeight-double-) | Sets the weight of the border line of a picture in units of pt. |
| [setBottom(int value)](#setBottom-int-) | Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels. |
| [setCreateId(UUID value)](#setCreateId-java.util.UUID-) | Sets create id for this shape. |
| [setData(byte[] value)](#setData-byte---) | Gets the data of the picture. |
| [setDisplayAsIcon(boolean value)](#setDisplayAsIcon-boolean-) | True if the specified object is displayed as an icon and the image will not be auto changed. |
| [setDynamicDataExchange(boolean value)](#setDynamicDataExchange-boolean-) | Sets whether dynamic data exchange |
| [setFilled(boolean value)](#setFilled-boolean-) | Indicates whether the fill format is visible. |
| [setFlippedHorizontally(boolean value)](#setFlippedHorizontally-boolean-) | Sets whether shape is horizontally flipped . |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | Sets whether shape is vertically flipped . |
| [setFont(Font value)](#setFont-com.aspose.cells.Font-) | Represents the font of shape. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Sets the data of the formula. |
| [setHasLine(boolean value)](#setHasLine-boolean-) | Sets the line border of the shape is visible. |
| [setHeight(int value)](#setHeight-int-) | Represents the height of shape, in unit of pixel. |
| [setHeightCM(double value)](#setHeightCM-double-) | Represents the height of the shape, in unit of centimeters. |
| [setHeightInChart(int value)](#setHeightInChart-int-) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. |
| [setHeightInShape(int value)](#setHeightInShape-int-) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. |
| [setHeightInch(double value)](#setHeightInch-double-) | Represents the height of the shape, in unit of inches. |
| [setHeightPt(double value)](#setHeightPt-double-) | Represents the height of the shape, in unit of points. |
| [setHeightScale(int value)](#setHeightScale-int-) | Sets the height scale,in unit of percent of the original picture height. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indicates whether the object is visible. |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | Sets the html string which contains data and some formats in this textbox. |
| [setInputRange(String value)](#setInputRange-java.lang.String-) | Sets the worksheet range used to fill the specified combo box. |
| [setInputRange(String formula, boolean isR1C1, boolean isLocal)](#setInputRange-java.lang.String-boolean-boolean-) | Sets the range used to fill the control. |
| [setLeft(int value)](#setLeft-int-) | Represents the horizontal offset of shape from its left column, in unit of pixels. |
| [setLeftCM(double value)](#setLeftCM-double-) | Represents the horizontal offset of shape from its left column, in unit of centimeters. |
| [setLeftInChart(int value)](#setLeftInChart-int-) | Represents the vertical offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. |
| [setLeftInShape(int value)](#setLeftInShape-int-) | Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. |
| [setLeftInch(double value)](#setLeftInch-double-) | Represents the horizontal offset of shape from its left column, in unit of inches. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Sets the horizonal offset of shape from worksheet left border. |
| [setLink(boolean value)](#setLink-boolean-) | Returns true if the picture is linked to a file. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Sets the worksheet range linked to the control's value. |
| [setLinkedCell(String formula, boolean isR1C1, boolean isLocal)](#setLinkedCell-java.lang.String-boolean-boolean-) | Sets the range linked to the control's value. |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) | True means that don't allow changes in aspect ratio. |
| [setLocked(boolean value)](#setLocked-boolean-) | True if the object is locked, False if the object can be modified when the sheet is protected. |
| [setLockedProperty(int type, boolean value)](#setLockedProperty-int-boolean-) | Set the locked property. |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | Sets the shape's horizontal offset from its lower right corner column. |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | Sets the shape's vertical offset from its lower right corner row. |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | Represents lower right corner column index. |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | Represents lower right corner row index. |
| [setMacroName(String value)](#setMacroName-java.lang.String-) | Sets the name of macro. |
| [setName(String value)](#setName-java.lang.String-) | Sets the name of the shape. |
| [setPlacement(int value)](#setPlacement-int-) | Represents the way the drawing object is attached to the cells below it. |
| [setPositionX(int value)](#setPositionX-int-) | Sets the horizonal offset of shape from worksheet left border,in unit of pixels. |
| [setPositionY(int value)](#setPositionY-int-) | Sets the vertical offset of shape from worksheet top border,in unit of pixels. |
| [setPrintable(boolean value)](#setPrintable-boolean-) | True if the object is printable |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | Indicates whether shape is relative to original picture size. |
| [setRight(int value)](#setRight-int-) | Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Sets the rotation of the shape. |
| [setSignatureLine(SignatureLine value)](#setSignatureLine-com.aspose.cells.SignatureLine-) | Sets the signature line |
| [setSoftEdges(double value)](#setSoftEdges-double-) | Sets the radius of blur to apply to the edges, in unit of points. |
| [setSourceFullName(String value)](#setSourceFullName-java.lang.String-) | Sets the path and name of the source file for the linked image. |
| [setText(String value)](#setText-java.lang.String-) | Represents the string in this TextBox object. |
| [setTextDirection(int value)](#setTextDirection-int-) | Sets the direction of the text flow for this object. |
| [setTextHorizontalAlignment(int value)](#setTextHorizontalAlignment-int-) | Sets the text horizontal alignment type of the shape. |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | Sets the text horizontal overflow type of the shape which contains text. |
| [setTextOptions(TextOptions value)](#setTextOptions-com.aspose.cells.TextOptions-) | Represents the text options of the shape. |
| [setTextOrientationType(int value)](#setTextOrientationType-int-) | Sets the text orientation type of the shape. |
| [setTextShapeType(int value)](#setTextShapeType-int-) | Sets the preset text shape type. |
| [setTextVerticalAlignment(int value)](#setTextVerticalAlignment-int-) | Sets the text vertical alignment type of the shape. |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | Sets the text vertical overflow type of the shape which contains text. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Sets the text wrapped type of the shape which contains text. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Specifies the title (caption) of the current shape object. |
| [setTop(int value)](#setTop-int-) | Represents the vertical offset of shape from its top row, in unit of pixels. |
| [setTopCM(double value)](#setTopCM-double-) | Represents the vertical offset of shape from its top row, in unit of centimeters. |
| [setTopInChart(int value)](#setTopInChart-int-) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. |
| [setTopInShape(int value)](#setTopInShape-int-) | Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. |
| [setTopInch(double value)](#setTopInch-double-) | Represents the vertical offset of shape from its top row, in unit of inches. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Sets the vertical offset of shape from worksheet top border, in unit of pixels. |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | Sets the shape's horizontal offset from its upper left corner column. |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | Sets the shape's vertical offset from its upper left corner row. |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | Represents upper left corner column index. |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | Represents upper left corner row index. |
| [setWidth(int value)](#setWidth-int-) | Represents the width of shape, in unit of pixels. |
| [setWidthCM(double value)](#setWidthCM-double-) | Represents the width of the shape, in unit of centimeters. |
| [setWidthInChart(int value)](#setWidthInChart-int-) | Represents the width of the shape, in unit of 1/4000 of the parent shape. |
| [setWidthInShape(int value)](#setWidthInShape-int-) | Represents the width of the shape, in unit of 1/4000 of the parent shape. |
| [setWidthInch(double value)](#setWidthInch-double-) | Represents the width of the shape, in unit of inch. |
| [setWidthPt(double value)](#setWidthPt-double-) | Represents the width of the shape, in unit of point. |
| [setWidthScale(int value)](#setWidthScale-int-) | Sets the width scale, in unit of percent of the original picture width. |
| [setX(int value)](#setX-int-) | Sets the horizontal offset of shape from worksheet left border,in unit of pixels. |
| [setY(int value)](#setY-int-) | Sets the vertical offset of shape from worksheet top border,in unit of pixels. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Returns the position of a shape in the z-order. |
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

**Example**

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

**Example**

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

**Example**

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

**Example**

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
### copy(Picture source, CopyOptions options) {#copy-com.aspose.cells.Picture-com.aspose.cells.CopyOptions-}
```
public void copy(Picture source, CopyOptions options)
```


Copy the picture.

**Example**

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //insert first picture
         int imgIndex1 = worksheet.getPictures().add(1, 1, "1.png");
         //Get the inserted picture object
         Picture pic1 = worksheet.getPictures().get(imgIndex1);
         //insert second picture
         int imgIndex2 = worksheet.getPictures().add(1, 9, "2.jpeg");
         //Get the inserted picture object
         Picture pic2 = worksheet.getPictures().get(imgIndex2);
         //Copy picture 1 to picture 2.You'll get two picture 1 objects that are superimposed on top of each other.
         CopyOptions opt = new CopyOptions();
         pic2.copy(pic1, opt);
         //Save the excel file.
         workbook.save("result.xlsx");
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [Picture](../../com.aspose.cells/picture) | The source picture. |
| options | [CopyOptions](../../com.aspose.cells/copyoptions) | The copy options. |

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

**Example**

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

**Example**

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

**Example**

```
shape.setAlternativeText("a rectangle");
```

**Returns:**
java.lang.String
### getAnchorType() {#getAnchorType--}
```
public int getAnchorType()
```


Gets the shape anchor placeholder. [ShapeAnchorType](../../com.aspose.cells/shapeanchortype).

**Example**

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


Gets the auto shape type. [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

```
if (shape.getAutoShapeType() == com.aspose.cells.AutoShapeType.UNKNOWN)
             shape.setAutoShapeType(com.aspose.cells.AutoShapeType.RECTANGLE);
```

**Returns:**
int
### getBorderLineColor() {#getBorderLineColor--}
```
public Color getBorderLineColor()
```


Represents the [Color](../../com.aspose.cells/color) of the border line of a picture.

**Example**

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
         int imgIndex = worksheet.getPictures().add(1, 1, "example.jpeg");
         //Get the inserted picture object
         Picture pic = worksheet.getPictures().get(imgIndex);
         //Set the border color of the picture
         pic.setBorderLineColor(Color.getRed());
         //Save the excel file.
         workbook.save("result.xlsx");
```

**Returns:**
[Color](../../com.aspose.cells/color)
### getBorderWeight() {#getBorderWeight--}
```
public double getBorderWeight()
```


Gets the weight of the border line of a picture in units of pt.

**Example**

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
         int imgIndex = worksheet.getPictures().add(1, 1, "example.jpeg");
         //Get the inserted picture object
         Picture pic = worksheet.getPictures().get(imgIndex);
         //Set the border color of the picture
         pic.setBorderLineColor(Color.getRed());
         //Set the border width of the picture
         pic.setBorderWeight(3);
         //Save the excel file.
         workbook.save("result.xlsx");
```

**Returns:**
double
### getBottom() {#getBottom--}
```
public int getBottom()
```


Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels.

**Example**

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

**Example**

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
### getConnectionPoints() {#getConnectionPoints--}
```
public float[][] getConnectionPoints()
```


Get the connection points

**Example**

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

**Example**

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


Gets create id for this shape.

**Returns:**
java.util.UUID
### getData() {#getData--}
```
public byte[] getData()
```


Gets the data of the picture.

**Example**

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //insert first picture
         int imgIndex1 = worksheet.getPictures().add(1, 1, "example1.png");
         //Get the inserted picture object
         Picture pic1 = worksheet.getPictures().get(imgIndex1);
         //insert second picture
         int imgIndex2 = worksheet.getPictures().add(1, 9, "example2.jpeg");
         //Get the inserted picture object
         Picture pic2 = worksheet.getPictures().get(imgIndex2);
         //Assign the byte data of the first image to the second image
         pic2.setData(pic1.getData());
         //Save the excel file.
         workbook.save("result.xlsx");
```

**Returns:**
byte[]
### getDisplayAsIcon() {#getDisplayAsIcon--}
```
public boolean getDisplayAsIcon()
```


True if the specified object is displayed as an icon and the image will not be auto changed.

**Returns:**
boolean
### getFill() {#getFill--}
```
public FillFormat getFill()
```


Returns a [Area.getFillFormat()](../../com.aspose.cells/area\#getFillFormat--) object that contains fill formatting properties for the specified shape.

**Example**

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

**Example**

```
Font font = shape.getFont();
         font.setName("Arial");
         font.setSize(12);
         font.setColor(Color.getRed());
```

**Returns:**
[Font](../../com.aspose.cells/font)
### getFormatPicture() {#getFormatPicture--}
```
public MsoFormatPicture getFormatPicture()
```


Gets the options of the picture format.

**Example**

```
MsoFormatPicture msoFormatPicture = shape.getFormatPicture();
```

**Returns:**
[MsoFormatPicture](../../com.aspose.cells/msoformatpicture)
### getFormula() {#getFormula--}
```
public String getFormula()
```


Gets the data of the formula.

**Returns:**
java.lang.String
### getGeometry() {#getGeometry--}
```
public Geometry getGeometry()
```


Gets the geometry

**Example**

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


Represents a [ShapePropertyCollection.getGlowEffect()](../../com.aspose.cells/shapepropertycollection\#getGlowEffect--) object that specifies glow effect for the chart element or shape.

**Example**

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

**Example**

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

**Example**

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

**Example**

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

**Example**

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

**Example**

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

**Example**

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


Gets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100;

**Example**

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


Gets the html string which contains data and some formats in this textbox.

**Example**

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

**Example**

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

**Example**

```
int id = shape.getId();
```

**Returns:**
int
### getImageType() {#getImageType--}
```
public int getImageType()
```


Gets the image format of the picture. [ImageOrPrintOptions.getImageType()](../../com.aspose.cells/imageorprintoptions\#getImageType--).

**Example**

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //insert first picture
         int imgIndex1 = worksheet.getPictures().add(1, 1, "1.png");
         //Get the inserted picture object
         Picture pic1 = worksheet.getPictures().get(imgIndex1);
         if(pic1.getImageType() == com.aspose.cells.ImageType.PNG)
         {
             //The picture's type is png.";
         }
         //insert second picture
         int imgIndex2 = worksheet.getPictures().add(1, 9, "2.jpeg");
         //Get the inserted picture object
         Picture pic2 = worksheet.getPictures().get(imgIndex2);
         if(pic2.getImageType() == com.aspose.cells.ImageType.JPEG)
         {
             //The picture's type is jpg.";
         }
```

**Returns:**
int
### getInputRange() {#getInputRange--}
```
public String getInputRange()
```


Gets the worksheet range used to fill the specified combo box.

**Example**

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

**Example**

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

**Example**

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

**Example**

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

**Example**

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

**Example**

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


Gets the horizonal offset of shape from worksheet left border.

**Example**

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

**Example**

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


Gets the worksheet range linked to the control's value.

**Example**

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

**Example**

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

**Example**

```
int noAdjustHandles = 0;
         if (shape.getLockedProperty(ShapeLockType.ADJUST_HANDLES))
             noAdjustHandles = 1;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [ShapeLockType](../../com.aspose.cells/shapelocktype). The type of the shape locked property. |

**Returns:**
boolean - Returns the value of locked property.
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```


Gets the shape's horizontal offset from its lower right corner column. The range of value is 0 to 1024.

**Example**

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


Gets the shape's vertical offset from its lower right corner row. The range of value is 0 to 256.

**Example**

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

**Example**

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

**Example**

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


Gets the name of macro.

**Example**

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


Gets mso drawing type. [MsoDrawingType](../../com.aspose.cells/msodrawingtype).

**Example**

```
/*Aspose.Cells.Drawing.MsoDrawingType*/int msoDrawingType = shape.getMsoDrawingType();
```

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Gets the name of the shape.

**Example**

```
shape.setName("shape1");
```

**Returns:**
java.lang.String
### getOriginalHeight() {#getOriginalHeight--}
```
public int getOriginalHeight()
```


Gets the original height of the picture.

**Example**

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
         int imgIndex = worksheet.getPictures().add(1, 1, "example.jpeg");
         //Get the inserted picture object
         Picture pic = worksheet.getPictures().get(imgIndex);
         //Gets the original height of the picture.
         int picHeight = pic.getOriginalHeight();
         //Save the excel file.
         workbook.save("result.xlsx");
```

**Returns:**
int
### getOriginalHeightCM() {#getOriginalHeightCM--}
```
public double getOriginalHeightCM()
```


Gets the original height of picture, in unit of centimeters.

**Example**

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
         int imgIndex = worksheet.getPictures().add(1, 1, "example.jpeg");
         //Get the inserted picture object
         Picture pic = worksheet.getPictures().get(imgIndex);
         //Gets the original height of the picture.
         double picHeightCM = pic.getOriginalHeightCM();
         //Save the excel file.
         workbook.save("result.xlsx");
```

**Returns:**
double
### getOriginalHeightInch() {#getOriginalHeightInch--}
```
public double getOriginalHeightInch()
```


Gets the original height of picture, in unit of inches.

**Example**

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
         int imgIndex = worksheet.getPictures().add(1, 1, "example.jpeg");
         //Get the inserted picture object
         Picture pic = worksheet.getPictures().get(imgIndex);
         //Gets the original height of the picture.
         double picHeightInch = pic.getOriginalHeightInch();
         //Save the excel file.
         workbook.save("result.xlsx");
```

**Returns:**
double
### getOriginalWidth() {#getOriginalWidth--}
```
public int getOriginalWidth()
```


Gets the original width of the picture.

**Example**

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
         int imgIndex = worksheet.getPictures().add(1, 1, "example.jpeg");
         //Get the inserted picture object
         Picture pic = worksheet.getPictures().get(imgIndex);
         //Gets the original width of the picture.
         int picWidth = pic.getOriginalWidth();
         //Save the excel file.
         workbook.save("result.xlsx");
```

**Returns:**
int
### getOriginalWidthCM() {#getOriginalWidthCM--}
```
public double getOriginalWidthCM()
```


Gets the original width of picture, in unit of centimeters.

**Example**

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
         int imgIndex = worksheet.getPictures().add(1, 1, "example.jpeg");
         //Get the inserted picture object
         Picture pic = worksheet.getPictures().get(imgIndex);
         //Gets the original width of the picture.
         double picWidthCM = pic.getOriginalWidthCM();
         //Save the excel file.
         workbook.save("result.xlsx");
```

**Returns:**
double
### getOriginalWidthInch() {#getOriginalWidthInch--}
```
public double getOriginalWidthInch()
```


Gets the original width of picture, in unit of inches.

**Example**

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
         int imgIndex = worksheet.getPictures().add(1, 1, "example.jpeg");
         //Get the inserted picture object
         Picture pic = worksheet.getPictures().get(imgIndex);
         //Gets the original width of the picture.
         double picWidthInch = pic.getOriginalWidthInch();
         //Save the excel file.
         workbook.save("result.xlsx");
```

**Returns:**
double
### getPaths() {#getPaths--}
```
public ShapePathCollection getPaths()
```


Gets the paths of a custom geometric shape.

**Example**

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


Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. [PlacementType](../../com.aspose.cells/placementtype).

**Example**

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


Gets the horizonal offset of shape from worksheet left border,in unit of pixels. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Drawing.Shape.X property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getPositionY() {#getPositionY--}
```
public int getPositionY()
```


Gets the vertical offset of shape from worksheet top border,in unit of pixels. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Drawing.Shape.Y property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getReflection() {#getReflection--}
```
public ReflectionEffect getReflection()
```


Represents a [ReflectionEffect](../../com.aspose.cells/reflectioneffect) object that specifies reflection effect for the chart element or shape.

**Example**

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

**Example**

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

**Example**

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

**Example**

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


Gets the rotation of the shape.

**Example**

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

**Example**

```
ShadowEffect shadowEffect = shape.getShadowEffect();
```

**Returns:**
[ShadowEffect](../../com.aspose.cells/shadoweffect)
### getSignatureLine() {#getSignatureLine--}
```
public SignatureLine getSignatureLine()
```


Gets the signature line

**Example**

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
         int imgIndex = worksheet.getPictures().add(1, 1, "example.jpeg");
         //Get the inserted picture object
         Picture pic = worksheet.getPictures().get(imgIndex);
         // Create signature line object
         SignatureLine s = new SignatureLine();
         s.setSigner("Simon Zhao");
         s.setTitle("Development Lead");
         s.setEmail("Simon.Zhao@aspose.com");
         // Assign the signature line object to Picture.
         pic.setSignatureLine(s);
         //Save the excel file.
         workbook.save("result.xlsx");
```

**Returns:**
[SignatureLine](../../com.aspose.cells/signatureline)
### getSoftEdges() {#getSoftEdges--}
```
public double getSoftEdges()
```


Gets the radius of blur to apply to the edges, in unit of points.

**Example**

```
shape.setSoftEdges(0.5d);
```

**Returns:**
double
### getSourceFullName() {#getSourceFullName--}
```
public String getSourceFullName()
```


Gets the path and name of the source file for the linked image. The default value is an empty string. If SourceFullName is not an empty string, the image is linked. If SourceFullName is not an empty string, but Data is null, then the image is linked and not stored in the file.

**Returns:**
java.lang.String
### getSpid() {#getSpid--}
```
public String getSpid()
```


Specifies an optional string that an application can use to Identify the particular shape.

**Example**

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

**Example**

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

**Example**

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


Gets the setting of the shape's text.

**Example**

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


Gets the direction of the text flow for this object. [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Example**

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

**Example**

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


Gets the text horizontal alignment type of the shape. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Example**

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


Gets the text horizontal overflow type of the shape which contains text. [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Example**

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

**Example**

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


Gets the text orientation type of the shape. [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Example**

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


Gets the preset text shape type. [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

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


Gets the text vertical alignment type of the shape. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Example**

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


Gets the text vertical overflow type of the shape which contains text. [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Example**

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


Gets 3d format of the shape.

**Example**

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

**Example**

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

**Example**

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

**Example**

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

**Example**

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

**Example**

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


Gets the vertical offset of shape from worksheet top border, in unit of pixels.

**Example**

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


Gets the auto shape type. [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

```
/*Aspose.Cells.Drawing.AutoShapeType*/int autoShapeType = shape.getType();
```

**Returns:**
int
### getUpperDeltaX() {#getUpperDeltaX--}
```
public int getUpperDeltaX()
```


Gets the shape's horizontal offset from its upper left corner column. The range of value is 0 to 1024.

**Example**

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


Gets the shape's vertical offset from its upper left corner row. The range of value is 0 to 256.

**Example**

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

**Example**

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

**Example**

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

**Example**

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

**Example**

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

**Example**

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

**Example**

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

**Example**

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


Gets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100;

**Example**

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

**Example**

```
Worksheet worksheet = shape.getWorksheet();
```

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
### getX() {#getX--}
```
public int getX()
```


Gets the horizontal offset of shape from worksheet left border,in unit of pixels.

**Example**

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


Gets the vertical offset of shape from worksheet top border,in unit of pixels.

**Example**

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

**Example**

```
shape.setZOrderPosition(3);
```

**Returns:**
int
### hasLine() {#hasLine--}
```
public boolean hasLine()
```


Gets the line border of the shape is visible.

**Example**

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
### isAutoSize() {#isAutoSize--}
```
public boolean isAutoSize()
```


True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated.

**Returns:**
boolean
### isDynamicDataExchange() {#isDynamicDataExchange--}
```
public boolean isDynamicDataExchange()
```


Gets whether dynamic data exchange

**Returns:**
boolean
### isEquation() {#isEquation--}
```
public boolean isEquation()
```


Indicates whether the shape only contains an equation.

**Example**

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

**Example**

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


Gets whether shape is horizontally flipped .

**Example**

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


Gets whether shape is vertically flipped .

**Example**

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

**Example**

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

**Example**

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
### isLink() {#isLink--}
```
public boolean isLink()
```


Returns true if the picture is linked to a file.

**Returns:**
boolean
### isLockAspectRatio() {#isLockAspectRatio--}
```
public boolean isLockAspectRatio()
```


True means that don't allow changes in aspect ratio.

**Example**

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

**Example**

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

**Example**

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

**Example**

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

**Example**

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //insert first picture
         int imgIndex1 = worksheet.getPictures().add(1, 1, "1.png");
         //Get the inserted picture object
         Picture pic1 = worksheet.getPictures().get(imgIndex1);
         //insert second picture
         int imgIndex2 = worksheet.getPictures().add(1, 9, "2.jpeg");
         //Get the inserted picture object
         Picture pic2 = worksheet.getPictures().get(imgIndex2);
         if(pic1.isSameSetting(pic1))
         {
             //two image objects are the same.
         }
 
         if(!pic1.isSameSetting(pic2))
         {
             //two image objects are not the same.
         }
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

**Example**

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


Gets the text wrapped type of the shape which contains text.

**Example**

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

**Example**

```
if(shape.isWordArt())
         {
             //This shape is a WordArt object.
         }
```

**Returns:**
boolean
### move(int upperLeftRow, int upperLeftColumn) {#move-int-int-}
```
public void move(int upperLeftRow, int upperLeftColumn)
```


Moves the picture to a specified location.

**Example**

```
//Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
         int imgIndex = worksheet.getPictures().add(1, 1, "example.jpeg");
         //Get the inserted picture object
         Picture pic = worksheet.getPictures().get(imgIndex);
         //Set the new location of the picture
         pic.move(2, 4);
         //Save the excel file.
         workbook.save("result.xlsx");
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int | Upper left row index. |
| upperLeftColumn | int | Upper left column index. |

### moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn) {#moveToRange-int-int-int-int-}
```
public void moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)
```


Moves the shape to a specified range.

**Example**

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

**Example**

```
shape.removeActiveXControl();
```

### removeHyperlink() {#removeHyperlink--}
```
public void removeHyperlink()
```


Remove the hyperlink of the shape.

**Example**

```
shape.removeHyperlink();
```

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


Returns or sets the descriptive (alternative) text string of the [Shape](../../com.aspose.cells/shape) object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setAnchorType(int value) {#setAnchorType-int-}
```
public void setAnchorType(int value)
```


Sets the shape anchor placeholder. [ShapeAnchorType](../../com.aspose.cells/shapeanchortype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setAutoShapeType(int value) {#setAutoShapeType-int-}
```
public void setAutoShapeType(int value)
```


Sets the auto shape type. [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


True indicates that the size of the ole object will be auto changed as the size of snapshot of the embedded content when the ole object is activated.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setBorderLineColor(Color value) {#setBorderLineColor-com.aspose.cells.Color-}
```
public void setBorderLineColor(Color value)
```


Represents the [Color](../../com.aspose.cells/color) of the border line of a picture.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setBorderWeight(double value) {#setBorderWeight-double-}
```
public void setBorderWeight(double value)
```


Sets the weight of the border line of a picture in units of pt.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setBottom(int value) {#setBottom-int-}
```
public void setBottom(int value)
```


Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCreateId(UUID value) {#setCreateId-java.util.UUID-}
```
public void setCreateId(UUID value)
```


Sets create id for this shape.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.UUID |  |

### setData(byte[] value) {#setData-byte---}
```
public void setData(byte[] value)
```


Gets the data of the picture.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte[] |  |

### setDisplayAsIcon(boolean value) {#setDisplayAsIcon-boolean-}
```
public void setDisplayAsIcon(boolean value)
```


True if the specified object is displayed as an icon and the image will not be auto changed.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDynamicDataExchange(boolean value) {#setDynamicDataExchange-boolean-}
```
public void setDynamicDataExchange(boolean value)
```


Sets whether dynamic data exchange

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFilled(boolean value) {#setFilled-boolean-}
```
public void setFilled(boolean value)
```


Indicates whether the fill format is visible.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFlippedHorizontally(boolean value) {#setFlippedHorizontally-boolean-}
```
public void setFlippedHorizontally(boolean value)
```


Sets whether shape is horizontally flipped .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```


Sets whether shape is vertically flipped .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setFont(Font value) {#setFont-com.aspose.cells.Font-}
```
public void setFont(Font value)
```


Represents the font of shape.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Font](../../com.aspose.cells/font) |  |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


Sets the data of the formula.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setHasLine(boolean value) {#setHasLine-boolean-}
```
public void setHasLine(boolean value)
```


Sets the line border of the shape is visible.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


Represents the height of shape, in unit of pixel.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


Represents the height of the shape, in unit of centimeters.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setHeightInChart(int value) {#setHeightInChart-int-}
```
public void setHeightInChart(int value)
```


Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Drawing.Shape.HeightInShape property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHeightInShape(int value) {#setHeightInShape-int-}
```
public void setHeightInShape(int value)
```


Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape.. Only Applies when this shape in the group or chart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


Represents the height of the shape, in unit of inches.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setHeightPt(double value) {#setHeightPt-double-}
```
public void setHeightPt(double value)
```


Represents the height of the shape, in unit of points.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setHeightScale(int value) {#setHeightScale-int-}
```
public void setHeightScale(int value)
```


Sets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100;

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Indicates whether the object is visible.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHtmlText(String value) {#setHtmlText-java.lang.String-}
```
public void setHtmlText(String value)
```


Sets the html string which contains data and some formats in this textbox.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setInputRange(String value) {#setInputRange-java.lang.String-}
```
public void setInputRange(String value)
```


Sets the worksheet range used to fill the specified combo box.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setInputRange(String formula, boolean isR1C1, boolean isLocal) {#setInputRange-java.lang.String-boolean-boolean-}
```
public void setInputRange(String formula, boolean isR1C1, boolean isLocal)
```


Sets the range used to fill the control.

**Example**

```
//After executing the code below, a ListBox object is created in the generated file. When the selected option is clicked, the selected value is displayed in cell A12.
 
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


Represents the horizontal offset of shape from its left column, in unit of pixels.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLeftCM(double value) {#setLeftCM-double-}
```
public void setLeftCM(double value)
```


Represents the horizontal offset of shape from its left column, in unit of centimeters.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setLeftInChart(int value) {#setLeftInChart-int-}
```
public void setLeftInChart(int value)
```


Represents the vertical offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Drawing.Shape.LeftInShape property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLeftInShape(int value) {#setLeftInShape-int-}
```
public void setLeftInShape(int value)
```


Represents the horizontal offset of shape from the left border of the parent shape, in unit of 1/4000 of width of the parent shape. Only Applies when this shape in the group or chart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLeftInch(double value) {#setLeftInch-double-}
```
public void setLeftInch(double value)
```


Represents the horizontal offset of shape from its left column, in unit of inches.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setLeftToCorner(int value) {#setLeftToCorner-int-}
```
public void setLeftToCorner(int value)
```


Sets the horizonal offset of shape from worksheet left border.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLink(boolean value) {#setLink-boolean-}
```
public void setLink(boolean value)
```


Returns true if the picture is linked to a file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


Sets the worksheet range linked to the control's value.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setLinkedCell(String formula, boolean isR1C1, boolean isLocal) {#setLinkedCell-java.lang.String-boolean-boolean-}
```
public void setLinkedCell(String formula, boolean isR1C1, boolean isLocal)
```


Sets the range linked to the control's value.

**Example**

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


True means that don't allow changes in aspect ratio.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


True if the object is locked, False if the object can be modified when the sheet is protected.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLockedProperty(int type, boolean value) {#setLockedProperty-int-boolean-}
```
public void setLockedProperty(int type, boolean value)
```


Set the locked property.

**Example**

```
shape.setLockedProperty(ShapeLockType.ADJUST_HANDLES, true);
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [ShapeLockType](../../com.aspose.cells/shapelocktype). The locked type. |
| value | boolean | The value of the property. |

### setLowerDeltaX(int value) {#setLowerDeltaX-int-}
```
public void setLowerDeltaX(int value)
```


Sets the shape's horizontal offset from its lower right corner column. The range of value is 0 to 1024.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLowerDeltaY(int value) {#setLowerDeltaY-int-}
```
public void setLowerDeltaY(int value)
```


Sets the shape's vertical offset from its lower right corner row. The range of value is 0 to 256.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLowerRightColumn(int value) {#setLowerRightColumn-int-}
```
public void setLowerRightColumn(int value)
```


Represents lower right corner column index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLowerRightRow(int value) {#setLowerRightRow-int-}
```
public void setLowerRightRow(int value)
```


Represents lower right corner row index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setMacroName(String value) {#setMacroName-java.lang.String-}
```
public void setMacroName(String value)
```


Sets the name of macro.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Sets the name of the shape.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setPlacement(int value) {#setPlacement-int-}
```
public void setPlacement(int value)
```


Represents the way the drawing object is attached to the cells below it. The property controls the placement of an object on a worksheet. [PlacementType](../../com.aspose.cells/placementtype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPositionX(int value) {#setPositionX-int-}
```
public void setPositionX(int value)
```


Sets the horizonal offset of shape from worksheet left border,in unit of pixels. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Drawing.Shape.X property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPositionY(int value) {#setPositionY-int-}
```
public void setPositionY(int value)
```


Sets the vertical offset of shape from worksheet top border,in unit of pixels. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Drawing.Shape.Y property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPrintable(boolean value) {#setPrintable-boolean-}
```
public void setPrintable(boolean value)
```


True if the object is printable

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRelativeToOriginalPictureSize(boolean value) {#setRelativeToOriginalPictureSize-boolean-}
```
public void setRelativeToOriginalPictureSize(boolean value)
```


Indicates whether shape is relative to original picture size.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRight(int value) {#setRight-int-}
```
public void setRight(int value)
```


Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


Sets the rotation of the shape.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setSignatureLine(SignatureLine value) {#setSignatureLine-com.aspose.cells.SignatureLine-}
```
public void setSignatureLine(SignatureLine value)
```


Sets the signature line

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [SignatureLine](../../com.aspose.cells/signatureline) |  |

### setSoftEdges(double value) {#setSoftEdges-double-}
```
public void setSoftEdges(double value)
```


Sets the radius of blur to apply to the edges, in unit of points.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setSourceFullName(String value) {#setSourceFullName-java.lang.String-}
```
public void setSourceFullName(String value)
```


Sets the path and name of the source file for the linked image. The default value is an empty string. If SourceFullName is not an empty string, the image is linked. If SourceFullName is not an empty string, but Data is null, then the image is linked and not stored in the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


Represents the string in this TextBox object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Sets the direction of the text flow for this object. [TextDirectionType](../../com.aspose.cells/textdirectiontype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextHorizontalAlignment(int value) {#setTextHorizontalAlignment-int-}
```
public void setTextHorizontalAlignment(int value)
```


Sets the text horizontal alignment type of the shape. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```


Sets the text horizontal overflow type of the shape which contains text. [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextOptions(TextOptions value) {#setTextOptions-com.aspose.cells.TextOptions-}
```
public void setTextOptions(TextOptions value)
```


Represents the text options of the shape.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TextOptions](../../com.aspose.cells/textoptions) |  |

### setTextOrientationType(int value) {#setTextOrientationType-int-}
```
public void setTextOrientationType(int value)
```


Sets the text orientation type of the shape. [TextOrientationType](../../com.aspose.cells/textorientationtype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```


Sets the preset text shape type. [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextVerticalAlignment(int value) {#setTextVerticalAlignment-int-}
```
public void setTextVerticalAlignment(int value)
```


Sets the text vertical alignment type of the shape. [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```


Sets the text vertical overflow type of the shape which contains text. [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


Sets the text wrapped type of the shape which contains text.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


Specifies the title (caption) of the current shape object.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setTop(int value) {#setTop-int-}
```
public void setTop(int value)
```


Represents the vertical offset of shape from its top row, in unit of pixels. If the shape is in the chart, represents the vertical offset of shape from its top border.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTopCM(double value) {#setTopCM-double-}
```
public void setTopCM(double value)
```


Represents the vertical offset of shape from its top row, in unit of centimeters.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setTopInChart(int value) {#setTopInChart-int-}
```
public void setTopInChart(int value)
```


Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Drawing.Shape.TopInShape property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTopInShape(int value) {#setTopInShape-int-}
```
public void setTopInShape(int value)
```


Represents the vertical offset of shape from the top border of the parent shape, in unit of 1/4000 of height of the parent shape. Only Applies when this shape in the group or chart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTopInch(double value) {#setTopInch-double-}
```
public void setTopInch(double value)
```


Represents the vertical offset of shape from its top row, in unit of inches.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setTopToCorner(int value) {#setTopToCorner-int-}
```
public void setTopToCorner(int value)
```


Sets the vertical offset of shape from worksheet top border, in unit of pixels.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setUpperDeltaX(int value) {#setUpperDeltaX-int-}
```
public void setUpperDeltaX(int value)
```


Sets the shape's horizontal offset from its upper left corner column. The range of value is 0 to 1024.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setUpperDeltaY(int value) {#setUpperDeltaY-int-}
```
public void setUpperDeltaY(int value)
```


Sets the shape's vertical offset from its upper left corner row. The range of value is 0 to 256.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setUpperLeftColumn(int value) {#setUpperLeftColumn-int-}
```
public void setUpperLeftColumn(int value)
```


Represents upper left corner column index.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setUpperLeftRow(int value) {#setUpperLeftRow-int-}
```
public void setUpperLeftRow(int value)
```


Represents upper left corner row index. If the shape is in the shape or in the group , UpperLeftRow will be ignored.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


Represents the width of shape, in unit of pixels.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


Represents the width of the shape, in unit of centimeters.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWidthInChart(int value) {#setWidthInChart-int-}
```
public void setWidthInChart(int value)
```


Represents the width of the shape, in unit of 1/4000 of the parent shape. NOTE: This member is now obsolete. Instead, please use Aspose.Cells.Drawing.Shape.WidthInShape property. This property will be removed 12 months later since JANUARY 2012. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setWidthInShape(int value) {#setWidthInShape-int-}
```
public void setWidthInShape(int value)
```


Represents the width of the shape, in unit of 1/4000 of the parent shape. Only Applies when this shape in the group or chart.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


Represents the width of the shape, in unit of inch.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWidthPt(double value) {#setWidthPt-double-}
```
public void setWidthPt(double value)
```


Represents the width of the shape, in unit of point.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWidthScale(int value) {#setWidthScale-int-}
```
public void setWidthScale(int value)
```


Sets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100;

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Sets the horizontal offset of shape from worksheet left border,in unit of pixels.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Sets the vertical offset of shape from worksheet top border,in unit of pixels.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```


Returns the position of a shape in the z-order.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### toFrontOrBack(int orders) {#toFrontOrBack-int-}
```
public void toFrontOrBack(int orders)
```


Brings the shape to the front or sends the shape to back.

**Example**

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

**Example**

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

**Example**

```
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

