---
title: GridPicture
second_title: Aspose.Cells for Java API Reference
description: Encapsulates the object that represents a single picture in a spreadsheet.
type: docs
url: /java/com.aspose.gridweb/gridpicture/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
com.aspose.gridweb.IGridSave
```
public class GridPicture implements IGridSave
```

Encapsulates the object that represents a single picture in a spreadsheet.
## Methods

| Method | Description |
| --- | --- |
| [addHyperlink(String param_string)](#addHyperlink-java.lang.String-) | Adds a hyperlink to the shape. |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | Moves the picture to the top-right corner. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeText()](#getAlternativeText--) |  |
| [getBorderLineColor()](#getBorderLineColor--) | Represents the [Color](../../com.aspose.cells/color) of the border line of a picture. |
| [getBorderWeight()](#getBorderWeight--) | the weight of the border line of a picture in units of pt. |
| [getBottom()](#getBottom--) |  |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Gets the data of the picture. |
| [getHeight()](#getHeight--) | Represents the height of shape, in unit of pixel. |
| [getHeightCM()](#getHeightCM--) | Represents the height of the shape, in unit of inches. |
| [getHeightInch()](#getHeightInch--) | Represents the height of the shape, in unit of inches. |
| [getHeightPt()](#getHeightPt--) | Represents the height of the shape, in unit of points. |
| [getHeightScale()](#getHeightScale--) | the height scale,in unit of percent of the original picture height. |
| [getHtmlText()](#getHtmlText--) | the html string which contains data and some formattings in this textbox. |
| [getHyperlink()](#getHyperlink--) | Gets the hyperlink of the shape. |
| [getID()](#getID--) | the ID of the picture. |
| [getImageFormat()](#getImageFormat--) | Gets the image format of the picture. |
| [getLeft()](#getLeft--) | Represents the horizontal offset of shape from its left column, in unit of pixels. |
| [getLeftCM()](#getLeftCM--) | Represents the horizontal offset of shape from its left column, in unit of centimeters. |
| [getLeftInch()](#getLeftInch--) | Represents the horizontal offset of shape from its left column, in unit of inches. |
| [getLinkedCell()](#getLinkedCell--) | the worksheet range linked to the control's value. |
| [getLowerDeltaX()](#getLowerDeltaX--) | the shape's horizontal offset from its lower right corner column. |
| [getLowerDeltaY()](#getLowerDeltaY--) | the shape's vertical offset from its lower right corner row. |
| [getLowerRightColumn()](#getLowerRightColumn--) | Represents lower right corner column index. |
| [getLowerRightRow()](#getLowerRightRow--) | Represents lower right corner row index. |
| [getName()](#getName--) | the name of the shape. |
| [getOriginalHeight()](#getOriginalHeight--) | Gets the original height of the picture. |
| [getOriginalHeightCM()](#getOriginalHeightCM--) | Gets the original height of picture, in unit of centimeters. |
| [getOriginalHeightInch()](#getOriginalHeightInch--) | Gets the original height of picture, in unit of inches. |
| [getOriginalWidth()](#getOriginalWidth--) | Gets the original width of the picture. |
| [getOriginalWidthCM()](#getOriginalWidthCM--) | Gets the original width of picture, in unit of centimeters. |
| [getOriginalWidthInch()](#getOriginalWidthInch--) | Gets the original width of picture, in unit of inches. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | Indicates whether shape is relative to original picture size. |
| [getRight()](#getRight--) | Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels. |
| [getRotationAngle()](#getRotationAngle--) | the rotation of the shape. |
| [getSourceFullName()](#getSourceFullName--) | the path and name of the source file for the linked image. |
| [getText()](#getText--) | Represents the string in this TextBox object. |
| [getTitle()](#getTitle--) |  |
| [getTop()](#getTop--) | Represents the vertical offset of shape from its top row, in unit of pixels. |
| [getTopCM()](#getTopCM--) | Represents the vertical offset of shape from its top row, in unit of centimeters. |
| [getTopInch()](#getTopInch--) | Represents the vertical offset of shape from its top row, in unit of inches. |
| [getUpperDeltaX()](#getUpperDeltaX--) | the shape's horizontal offset from its upper left corner column. |
| [getUpperDeltaY()](#getUpperDeltaY--) | the shape's vertical offset from its upper left corner row. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Represents upper left corner column index. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Represents upper left corner row index. |
| [getWidth()](#getWidth--) | Represents the width of shape, in unit of pixels. |
| [getWidthCM()](#getWidthCM--) | Represents the width of the shape, in unit of centimeters. |
| [getWidthInch()](#getWidthInch--) | Represents the width of the shape, in unit of inch. |
| [getWidthPt()](#getWidthPt--) | Represents the width of the shape, in unit of point. |
| [getWidthScale()](#getWidthScale--) | the width scale, in unit of percent of the original picture width. |
| [getX()](#getX--) | the horizonal offset of shape from worksheet left border,in unit of pixels. |
| [getY()](#getY--) | the vertical offset of shape from worksheet top border,in unit of pixels. |
| [getZOrderPosition()](#getZOrderPosition--) | Returns the position of a shape in the z-order. |
| [hasLine()](#hasLine--) | the line border of the shape is visible. |
| [hashCode()](#hashCode--) |  |
| [isFlippedVertically()](#isFlippedVertically--) | whether shape is vertically flipped . |
| [isGroup()](#isGroup--) | Indicates whether the shape is a group. |
| [isHidden()](#isHidden--) | Indicates whether the object is visible. |
| [isLockAspectRatio()](#isLockAspectRatio--) | True means that don't allow changes in aspect ratio. |
| [isLocked()](#isLocked--) | True if the object is locked, False if the object can be modified when the sheet is protected. |
| [isTextWrapped()](#isTextWrapped--) | the text wrapped type of the shape which contains text. |
| [move(int upperLeftRow, int upperLeftColumn)](#move-int-int-) | Moves the picture to a specified location. |
| [moveToRange(int param0_int, int param1_int, int param2_int, int param3_int)](#moveToRange-int-int-int-int-) | Moves the shape to a specified range. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeHyperlink()](#removeHyperlink--) | Remove the hyperlink of the shape. |
| [saveToImage(InputStream s)](#saveToImage-java.io.InputStream-) | Creates the image and saves it to a stream . |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | For the description of this property, please see [getAlternativeText()](../../com.aspose.gridweb/gridpicture\#getAlternativeText--) |
| [setBorderLineColor(Color value)](#setBorderLineColor-com.aspose.gridweb.Color-) | For the description of this property, please see [getBorderLineColor()](../../com.aspose.gridweb/gridpicture\#getBorderLineColor--) |
| [setBorderWeight(double value)](#setBorderWeight-double-) | For the description of this property, please see [getBorderWeight()](../../com.aspose.gridweb/gridpicture\#getBorderWeight--) |
| [setBottom(int value)](#setBottom-int-) | For the description of this property, please see [getBottom()](../../com.aspose.gridweb/gridpicture\#getBottom--) |
| [setData(byte[] value)](#setData-byte---) | For the description of this property, please see [getData()](../../com.aspose.gridweb/gridpicture\#getData--) |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | For the description of this property, please see [isFlippedVertically()](../../com.aspose.gridweb/gridpicture\#isFlippedVertically--) |
| [setHasLine(boolean value)](#setHasLine-boolean-) | For the description of this property, please see [hasLine()](../../com.aspose.gridweb/gridpicture\#hasLine--) |
| [setHeight(int value)](#setHeight-int-) | For the description of this property, please see [getHeight()](../../com.aspose.gridweb/gridpicture\#getHeight--) |
| [setHeightCM(double value)](#setHeightCM-double-) | For the description of this property, please see [getHeightCM()](../../com.aspose.gridweb/gridpicture\#getHeightCM--) |
| [setHeightInch(double value)](#setHeightInch-double-) | For the description of this property, please see [getHeightInch()](../../com.aspose.gridweb/gridpicture\#getHeightInch--) |
| [setHeightPt(double value)](#setHeightPt-double-) | For the description of this property, please see [getHeightPt()](../../com.aspose.gridweb/gridpicture\#getHeightPt--) |
| [setHeightScale(int value)](#setHeightScale-int-) | For the description of this property, please see [getHeightScale()](../../com.aspose.gridweb/gridpicture\#getHeightScale--) |
| [setHidden(boolean value)](#setHidden-boolean-) | For the description of this property, please see [isHidden()](../../com.aspose.gridweb/gridpicture\#isHidden--) |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | For the description of this property, please see [getHtmlText()](../../com.aspose.gridweb/gridpicture\#getHtmlText--) |
| [setID(String value)](#setID-java.lang.String-) | For the description of this property, please see [getID()](../../com.aspose.gridweb/gridpicture\#getID--) |
| [setLeft(int value)](#setLeft-int-) | For the description of this property, please see [getLeft()](../../com.aspose.gridweb/gridpicture\#getLeft--) |
| [setLeftCM(double value)](#setLeftCM-double-) | For the description of this property, please see [getLeftCM()](../../com.aspose.gridweb/gridpicture\#getLeftCM--) |
| [setLeftInch(double value)](#setLeftInch-double-) | For the description of this property, please see [getLeftInch()](../../com.aspose.gridweb/gridpicture\#getLeftInch--) |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | For the description of this property, please see [getLinkedCell()](../../com.aspose.gridweb/gridpicture\#getLinkedCell--) |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) |  |
| [setLocked(boolean value)](#setLocked-boolean-) | For the description of this property, please see [isLocked()](../../com.aspose.gridweb/gridpicture\#isLocked--) |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | For the description of this property, please see [getLowerDeltaX()](../../com.aspose.gridweb/gridpicture\#getLowerDeltaX--) |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | For the description of this property, please see [getLowerDeltaY()](../../com.aspose.gridweb/gridpicture\#getLowerDeltaY--) |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | For the description of this property, please see [getLowerRightColumn()](../../com.aspose.gridweb/gridpicture\#getLowerRightColumn--) |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | For the description of this property, please see [getLowerRightRow()](../../com.aspose.gridweb/gridpicture\#getLowerRightRow--) |
| [setName(String value)](#setName-java.lang.String-) | For the description of this property, please see [getName()](../../com.aspose.gridweb/gridpicture\#getName--) |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | For the description of this property, please see [getRelativeToOriginalPictureSize()](../../com.aspose.gridweb/gridpicture\#getRelativeToOriginalPictureSize--) |
| [setRight(int value)](#setRight-int-) | For the description of this property, please see [getRight()](../../com.aspose.gridweb/gridpicture\#getRight--) |
| [setRotationAngle(double value)](#setRotationAngle-double-) | For the description of this property, please see [getRotationAngle()](../../com.aspose.gridweb/gridpicture\#getRotationAngle--) |
| [setSourceFullName(String value)](#setSourceFullName-java.lang.String-) | For the description of this property, please see [getSourceFullName()](../../com.aspose.gridweb/gridpicture\#getSourceFullName--) |
| [setText(String value)](#setText-java.lang.String-) | For the description of this property, please see [getText()](../../com.aspose.gridweb/gridpicture\#getText--) |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | For the description of this property, please see [isTextWrapped()](../../com.aspose.gridweb/gridpicture\#isTextWrapped--) |
| [setTitle(String value)](#setTitle-java.lang.String-) | For the description of this property, please see [getTitle()](../../com.aspose.gridweb/gridpicture\#getTitle--) |
| [setTop(int value)](#setTop-int-) | For the description of this property, please see [getTop()](../../com.aspose.gridweb/gridpicture\#getTop--) |
| [setTopCM(double value)](#setTopCM-double-) | For the description of this property, please see [getTopCM()](../../com.aspose.gridweb/gridpicture\#getTopCM--) |
| [setTopInch(double value)](#setTopInch-double-) | For the description of this property, please see [getTopInch()](../../com.aspose.gridweb/gridpicture\#getTopInch--) |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | For the description of this property, please see [getUpperDeltaX()](../../com.aspose.gridweb/gridpicture\#getUpperDeltaX--) |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | For the description of this property, please see [getUpperDeltaY()](../../com.aspose.gridweb/gridpicture\#getUpperDeltaY--) |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | For the description of this property, please see [getUpperLeftColumn()](../../com.aspose.gridweb/gridpicture\#getUpperLeftColumn--) |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | For the description of this property, please see [getUpperLeftRow()](../../com.aspose.gridweb/gridpicture\#getUpperLeftRow--) |
| [setWidth(int value)](#setWidth-int-) | For the description of this property, please see [getWidth()](../../com.aspose.gridweb/gridpicture\#getWidth--) |
| [setWidthCM(double value)](#setWidthCM-double-) | For the description of this property, please see [getWidthCM()](../../com.aspose.gridweb/gridpicture\#getWidthCM--) |
| [setWidthInch(double value)](#setWidthInch-double-) | For the description of this property, please see [getWidthInch()](../../com.aspose.gridweb/gridpicture\#getWidthInch--) |
| [setWidthPt(double value)](#setWidthPt-double-) | For the description of this property, please see [getWidthPt()](../../com.aspose.gridweb/gridpicture\#getWidthPt--) |
| [setWidthScale(int value)](#setWidthScale-int-) | For the description of this property, please see [getWidthScale()](../../com.aspose.gridweb/gridpicture\#getWidthScale--) |
| [setX(int value)](#setX-int-) | For the description of this property, please see [getX()](../../com.aspose.gridweb/gridpicture\#getX--) |
| [setY(int value)](#setY-int-) | For the description of this property, please see [getY()](../../com.aspose.gridweb/gridpicture\#getY--) |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | For the description of this property, please see [getZOrderPosition()](../../com.aspose.gridweb/gridpicture\#getZOrderPosition--) |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String param_string) {#addHyperlink-java.lang.String-}
```
public GridHyperlink addHyperlink(String param_string)
```


Adds a hyperlink to the shape.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| param_string | java.lang.String |  |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - Return the new hyperlink object.
### alignTopRightCorner(int topRow, int rightColumn) {#alignTopRightCorner-int-int-}
```
public void alignTopRightCorner(int topRow, int rightColumn)
```


Moves the picture to the top-right corner.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int | the row index. |
| rightColumn | int | the column index. |

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
### getAlternativeText() {#getAlternativeText--}
```
public String getAlternativeText()
```




**Returns:**
java.lang.String
### getBorderLineColor() {#getBorderLineColor--}
```
public Color getBorderLineColor()
```


Represents the [Color](../../com.aspose.cells/color) of the border line of a picture.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getBorderWeight() {#getBorderWeight--}
```
public double getBorderWeight()
```


the weight of the border line of a picture in units of pt.

**Returns:**
double
### getBottom() {#getBottom--}
```
public int getBottom()
```




**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getData() {#getData--}
```
public byte[] getData()
```


Gets the data of the picture.

**Returns:**
byte[]
### getHeight() {#getHeight--}
```
public int getHeight()
```


Represents the height of shape, in unit of pixel.

**Returns:**
int
### getHeightCM() {#getHeightCM--}
```
public double getHeightCM()
```


Represents the height of the shape, in unit of inches.

**Returns:**
double
### getHeightInch() {#getHeightInch--}
```
public double getHeightInch()
```


Represents the height of the shape, in unit of inches.

**Returns:**
double
### getHeightPt() {#getHeightPt--}
```
public double getHeightPt()
```


Represents the height of the shape, in unit of points.

**Returns:**
double
### getHeightScale() {#getHeightScale--}
```
public int getHeightScale()
```


the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100;

**Returns:**
int
### getHtmlText() {#getHtmlText--}
```
public String getHtmlText()
```


the html string which contains data and some formattings in this textbox.

**Returns:**
java.lang.String
### getHyperlink() {#getHyperlink--}
```
public GridHyperlink getHyperlink()
```


Gets the hyperlink of the shape.

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink)
### getID() {#getID--}
```
public String getID()
```


the ID of the picture.

**Returns:**
java.lang.String
### getImageFormat() {#getImageFormat--}
```
public int getImageFormat()
```


Gets the image format of the picture.

**Returns:**
int
### getLeft() {#getLeft--}
```
public int getLeft()
```


Represents the horizontal offset of shape from its left column, in unit of pixels.

**Returns:**
int
### getLeftCM() {#getLeftCM--}
```
public double getLeftCM()
```


Represents the horizontal offset of shape from its left column, in unit of centimeters.

**Returns:**
double
### getLeftInch() {#getLeftInch--}
```
public double getLeftInch()
```


Represents the horizontal offset of shape from its left column, in unit of inches.

**Returns:**
double
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```


the worksheet range linked to the control's value.

**Returns:**
java.lang.String
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```


the shape's horizontal offset from its lower right corner column. The range of value is 0 to 1024.

**Returns:**
int
### getLowerDeltaY() {#getLowerDeltaY--}
```
public int getLowerDeltaY()
```


the shape's vertical offset from its lower right corner row. The range of value is 0 to 256.

**Returns:**
int
### getLowerRightColumn() {#getLowerRightColumn--}
```
public int getLowerRightColumn()
```


Represents lower right corner column index.

**Returns:**
int
### getLowerRightRow() {#getLowerRightRow--}
```
public int getLowerRightRow()
```


Represents lower right corner row index.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


the name of the shape.

**Returns:**
java.lang.String
### getOriginalHeight() {#getOriginalHeight--}
```
public int getOriginalHeight()
```


Gets the original height of the picture.

**Returns:**
int
### getOriginalHeightCM() {#getOriginalHeightCM--}
```
public double getOriginalHeightCM()
```


Gets the original height of picture, in unit of centimeters.

**Returns:**
double
### getOriginalHeightInch() {#getOriginalHeightInch--}
```
public double getOriginalHeightInch()
```


Gets the original height of picture, in unit of inches.

**Returns:**
double
### getOriginalWidth() {#getOriginalWidth--}
```
public int getOriginalWidth()
```


Gets the original width of the picture.

**Returns:**
int
### getOriginalWidthCM() {#getOriginalWidthCM--}
```
public double getOriginalWidthCM()
```


Gets the original width of picture, in unit of centimeters.

**Returns:**
double
### getOriginalWidthInch() {#getOriginalWidthInch--}
```
public double getOriginalWidthInch()
```


Gets the original width of picture, in unit of inches.

**Returns:**
double
### getRelativeToOriginalPictureSize() {#getRelativeToOriginalPictureSize--}
```
public boolean getRelativeToOriginalPictureSize()
```


Indicates whether shape is relative to original picture size.

**Returns:**
boolean
### getRight() {#getRight--}
```
public int getRight()
```


Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels.

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


the rotation of the shape.

**Returns:**
double
### getSourceFullName() {#getSourceFullName--}
```
public String getSourceFullName()
```


the path and name of the source file for the linked image. The default value is an empty string. If SourceFullName is not an empty string, the image is linked. If SourceFullName is not an empty string, but Data is null, then the image is linked and not stored in the file.

**Returns:**
java.lang.String
### getText() {#getText--}
```
public String getText()
```


Represents the string in this TextBox object.

**Returns:**
java.lang.String
### getTitle() {#getTitle--}
```
public String getTitle()
```




**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```


Represents the vertical offset of shape from its top row, in unit of pixels. If the shape is in the chart, represents the vertical offset of shape from its top border.

**Returns:**
int
### getTopCM() {#getTopCM--}
```
public double getTopCM()
```


Represents the vertical offset of shape from its top row, in unit of centimeters.

**Returns:**
double
### getTopInch() {#getTopInch--}
```
public double getTopInch()
```


Represents the vertical offset of shape from its top row, in unit of inches.

**Returns:**
double
### getUpperDeltaX() {#getUpperDeltaX--}
```
public int getUpperDeltaX()
```


the shape's horizontal offset from its upper left corner column. The range of value is 0 to 1024.

**Returns:**
int
### getUpperDeltaY() {#getUpperDeltaY--}
```
public int getUpperDeltaY()
```


the shape's vertical offset from its upper left corner row. The range of value is 0 to 256.

**Returns:**
int
### getUpperLeftColumn() {#getUpperLeftColumn--}
```
public int getUpperLeftColumn()
```


Represents upper left corner column index.

**Returns:**
int
### getUpperLeftRow() {#getUpperLeftRow--}
```
public int getUpperLeftRow()
```


Represents upper left corner row index. If the shape is in the shape or in the group , UpperLeftRow will be ignored.

**Returns:**
int
### getWidth() {#getWidth--}
```
public int getWidth()
```


Represents the width of shape, in unit of pixels.

**Returns:**
int
### getWidthCM() {#getWidthCM--}
```
public double getWidthCM()
```


Represents the width of the shape, in unit of centimeters.

**Returns:**
double
### getWidthInch() {#getWidthInch--}
```
public double getWidthInch()
```


Represents the width of the shape, in unit of inch.

**Returns:**
double
### getWidthPt() {#getWidthPt--}
```
public double getWidthPt()
```


Represents the width of the shape, in unit of point.

**Returns:**
double
### getWidthScale() {#getWidthScale--}
```
public int getWidthScale()
```


the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100;

**Returns:**
int
### getX() {#getX--}
```
public int getX()
```


the horizonal offset of shape from worksheet left border,in unit of pixels.

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


the vertical offset of shape from worksheet top border,in unit of pixels.

**Returns:**
int
### getZOrderPosition() {#getZOrderPosition--}
```
public int getZOrderPosition()
```


Returns the position of a shape in the z-order.

**Returns:**
int
### hasLine() {#hasLine--}
```
public boolean hasLine()
```


the line border of the shape is visible.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isFlippedVertically() {#isFlippedVertically--}
```
public boolean isFlippedVertically()
```


whether shape is vertically flipped .

**Returns:**
boolean
### isGroup() {#isGroup--}
```
public boolean isGroup()
```


Indicates whether the shape is a group.

**Returns:**
boolean
### isHidden() {#isHidden--}
```
public boolean isHidden()
```


Indicates whether the object is visible.

**Returns:**
boolean
### isLockAspectRatio() {#isLockAspectRatio--}
```
public boolean isLockAspectRatio()
```


True means that don't allow changes in aspect ratio.

**Returns:**
boolean
### isLocked() {#isLocked--}
```
public boolean isLocked()
```


True if the object is locked, False if the object can be modified when the sheet is protected.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


the text wrapped type of the shape which contains text.

**Returns:**
boolean
### move(int upperLeftRow, int upperLeftColumn) {#move-int-int-}
```
public void move(int upperLeftRow, int upperLeftColumn)
```


Moves the picture to a specified location.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| upperLeftRow | int | Upper left row index. |
| upperLeftColumn | int | Upper left column index. |

### moveToRange(int param0_int, int param1_int, int param2_int, int param3_int) {#moveToRange-int-int-int-int-}
```
public void moveToRange(int param0_int, int param1_int, int param2_int, int param3_int)
```


Moves the shape to a specified range.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| param0_int | int |  |
| param1_int | int |  |
| param2_int | int |  |
| param3_int | int |  |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### removeHyperlink() {#removeHyperlink--}
```
public void removeHyperlink()
```


Remove the hyperlink of the shape.

### saveToImage(InputStream s) {#saveToImage-java.io.InputStream-}
```
public void saveToImage(InputStream s)
```


Creates the image and saves it to a stream .

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| s | java.io.InputStream |  |

### setAlternativeText(String value) {#setAlternativeText-java.lang.String-}
```
public void setAlternativeText(String value)
```


For the description of this property, please see [getAlternativeText()](../../com.aspose.gridweb/gridpicture\#getAlternativeText--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setBorderLineColor(Color value) {#setBorderLineColor-com.aspose.gridweb.Color-}
```
public void setBorderLineColor(Color value)
```


For the description of this property, please see [getBorderLineColor()](../../com.aspose.gridweb/gridpicture\#getBorderLineColor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setBorderWeight(double value) {#setBorderWeight-double-}
```
public void setBorderWeight(double value)
```


For the description of this property, please see [getBorderWeight()](../../com.aspose.gridweb/gridpicture\#getBorderWeight--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setBottom(int value) {#setBottom-int-}
```
public void setBottom(int value)
```


For the description of this property, please see [getBottom()](../../com.aspose.gridweb/gridpicture\#getBottom--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setData(byte[] value) {#setData-byte---}
```
public void setData(byte[] value)
```


For the description of this property, please see [getData()](../../com.aspose.gridweb/gridpicture\#getData--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte[] |  |

### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```


For the description of this property, please see [isFlippedVertically()](../../com.aspose.gridweb/gridpicture\#isFlippedVertically--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHasLine(boolean value) {#setHasLine-boolean-}
```
public void setHasLine(boolean value)
```


For the description of this property, please see [hasLine()](../../com.aspose.gridweb/gridpicture\#hasLine--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHeight(int value) {#setHeight-int-}
```
public void setHeight(int value)
```


For the description of this property, please see [getHeight()](../../com.aspose.gridweb/gridpicture\#getHeight--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHeightCM(double value) {#setHeightCM-double-}
```
public void setHeightCM(double value)
```


For the description of this property, please see [getHeightCM()](../../com.aspose.gridweb/gridpicture\#getHeightCM--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setHeightInch(double value) {#setHeightInch-double-}
```
public void setHeightInch(double value)
```


For the description of this property, please see [getHeightInch()](../../com.aspose.gridweb/gridpicture\#getHeightInch--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setHeightPt(double value) {#setHeightPt-double-}
```
public void setHeightPt(double value)
```


For the description of this property, please see [getHeightPt()](../../com.aspose.gridweb/gridpicture\#getHeightPt--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setHeightScale(int value) {#setHeightScale-int-}
```
public void setHeightScale(int value)
```


For the description of this property, please see [getHeightScale()](../../com.aspose.gridweb/gridpicture\#getHeightScale--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


For the description of this property, please see [isHidden()](../../com.aspose.gridweb/gridpicture\#isHidden--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setHtmlText(String value) {#setHtmlText-java.lang.String-}
```
public void setHtmlText(String value)
```


For the description of this property, please see [getHtmlText()](../../com.aspose.gridweb/gridpicture\#getHtmlText--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setID(String value) {#setID-java.lang.String-}
```
public void setID(String value)
```


For the description of this property, please see [getID()](../../com.aspose.gridweb/gridpicture\#getID--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setLeft(int value) {#setLeft-int-}
```
public void setLeft(int value)
```


For the description of this property, please see [getLeft()](../../com.aspose.gridweb/gridpicture\#getLeft--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLeftCM(double value) {#setLeftCM-double-}
```
public void setLeftCM(double value)
```


For the description of this property, please see [getLeftCM()](../../com.aspose.gridweb/gridpicture\#getLeftCM--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setLeftInch(double value) {#setLeftInch-double-}
```
public void setLeftInch(double value)
```


For the description of this property, please see [getLeftInch()](../../com.aspose.gridweb/gridpicture\#getLeftInch--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```


For the description of this property, please see [getLinkedCell()](../../com.aspose.gridweb/gridpicture\#getLinkedCell--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setLockAspectRatio(boolean value) {#setLockAspectRatio-boolean-}
```
public void setLockAspectRatio(boolean value)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLocked(boolean value) {#setLocked-boolean-}
```
public void setLocked(boolean value)
```


For the description of this property, please see [isLocked()](../../com.aspose.gridweb/gridpicture\#isLocked--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLowerDeltaX(int value) {#setLowerDeltaX-int-}
```
public void setLowerDeltaX(int value)
```


For the description of this property, please see [getLowerDeltaX()](../../com.aspose.gridweb/gridpicture\#getLowerDeltaX--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLowerDeltaY(int value) {#setLowerDeltaY-int-}
```
public void setLowerDeltaY(int value)
```


For the description of this property, please see [getLowerDeltaY()](../../com.aspose.gridweb/gridpicture\#getLowerDeltaY--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLowerRightColumn(int value) {#setLowerRightColumn-int-}
```
public void setLowerRightColumn(int value)
```


For the description of this property, please see [getLowerRightColumn()](../../com.aspose.gridweb/gridpicture\#getLowerRightColumn--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setLowerRightRow(int value) {#setLowerRightRow-int-}
```
public void setLowerRightRow(int value)
```


For the description of this property, please see [getLowerRightRow()](../../com.aspose.gridweb/gridpicture\#getLowerRightRow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


For the description of this property, please see [getName()](../../com.aspose.gridweb/gridpicture\#getName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setRelativeToOriginalPictureSize(boolean value) {#setRelativeToOriginalPictureSize-boolean-}
```
public void setRelativeToOriginalPictureSize(boolean value)
```


For the description of this property, please see [getRelativeToOriginalPictureSize()](../../com.aspose.gridweb/gridpicture\#getRelativeToOriginalPictureSize--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setRight(int value) {#setRight-int-}
```
public void setRight(int value)
```


For the description of this property, please see [getRight()](../../com.aspose.gridweb/gridpicture\#getRight--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


For the description of this property, please see [getRotationAngle()](../../com.aspose.gridweb/gridpicture\#getRotationAngle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setSourceFullName(String value) {#setSourceFullName-java.lang.String-}
```
public void setSourceFullName(String value)
```


For the description of this property, please see [getSourceFullName()](../../com.aspose.gridweb/gridpicture\#getSourceFullName--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


For the description of this property, please see [getText()](../../com.aspose.gridweb/gridpicture\#getText--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


For the description of this property, please see [isTextWrapped()](../../com.aspose.gridweb/gridpicture\#isTextWrapped--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setTitle(String value) {#setTitle-java.lang.String-}
```
public void setTitle(String value)
```


For the description of this property, please see [getTitle()](../../com.aspose.gridweb/gridpicture\#getTitle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setTop(int value) {#setTop-int-}
```
public void setTop(int value)
```


For the description of this property, please see [getTop()](../../com.aspose.gridweb/gridpicture\#getTop--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTopCM(double value) {#setTopCM-double-}
```
public void setTopCM(double value)
```


For the description of this property, please see [getTopCM()](../../com.aspose.gridweb/gridpicture\#getTopCM--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setTopInch(double value) {#setTopInch-double-}
```
public void setTopInch(double value)
```


For the description of this property, please see [getTopInch()](../../com.aspose.gridweb/gridpicture\#getTopInch--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setUpperDeltaX(int value) {#setUpperDeltaX-int-}
```
public void setUpperDeltaX(int value)
```


For the description of this property, please see [getUpperDeltaX()](../../com.aspose.gridweb/gridpicture\#getUpperDeltaX--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setUpperDeltaY(int value) {#setUpperDeltaY-int-}
```
public void setUpperDeltaY(int value)
```


For the description of this property, please see [getUpperDeltaY()](../../com.aspose.gridweb/gridpicture\#getUpperDeltaY--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setUpperLeftColumn(int value) {#setUpperLeftColumn-int-}
```
public void setUpperLeftColumn(int value)
```


For the description of this property, please see [getUpperLeftColumn()](../../com.aspose.gridweb/gridpicture\#getUpperLeftColumn--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setUpperLeftRow(int value) {#setUpperLeftRow-int-}
```
public void setUpperLeftRow(int value)
```


For the description of this property, please see [getUpperLeftRow()](../../com.aspose.gridweb/gridpicture\#getUpperLeftRow--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setWidth(int value) {#setWidth-int-}
```
public void setWidth(int value)
```


For the description of this property, please see [getWidth()](../../com.aspose.gridweb/gridpicture\#getWidth--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setWidthCM(double value) {#setWidthCM-double-}
```
public void setWidthCM(double value)
```


For the description of this property, please see [getWidthCM()](../../com.aspose.gridweb/gridpicture\#getWidthCM--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWidthInch(double value) {#setWidthInch-double-}
```
public void setWidthInch(double value)
```


For the description of this property, please see [getWidthInch()](../../com.aspose.gridweb/gridpicture\#getWidthInch--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWidthPt(double value) {#setWidthPt-double-}
```
public void setWidthPt(double value)
```


For the description of this property, please see [getWidthPt()](../../com.aspose.gridweb/gridpicture\#getWidthPt--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setWidthScale(int value) {#setWidthScale-int-}
```
public void setWidthScale(int value)
```


For the description of this property, please see [getWidthScale()](../../com.aspose.gridweb/gridpicture\#getWidthScale--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setX(int value) {#setX-int-}
```
public void setX(int value)
```


For the description of this property, please see [getX()](../../com.aspose.gridweb/gridpicture\#getX--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


For the description of this property, please see [getY()](../../com.aspose.gridweb/gridpicture\#getY--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setZOrderPosition(int value) {#setZOrderPosition-int-}
```
public void setZOrderPosition(int value)
```


For the description of this property, please see [getZOrderPosition()](../../com.aspose.gridweb/gridpicture\#getZOrderPosition--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
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

