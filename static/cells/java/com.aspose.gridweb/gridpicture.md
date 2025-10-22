##GridPicture
Encapsulates the object that represents a single picture in a spreadsheet.
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
| [addHyperlink(String address)](#addHyperlink-java.lang.String-) | Adds a hyperlink to the shape. |
| [alignTopRightCorner(int topRow, int rightColumn)](#alignTopRightCorner-int-int-) | Moves the picture to the top-right corner. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlternativeText()](#getAlternativeText--) | Returns or sets the descriptive (alternative) text string of the [GridShape](../../com.aspose.gridweb/gridshape) object. |
| [getBorderLineColor()](#getBorderLineColor--) | Represents the [Color](../../com.aspose.cells/color) of the border line of a picture. |
| [getBorderWeight()](#getBorderWeight--) | Gets the weight of the border line of a picture in units of pt. |
| [getBottom()](#getBottom--) | Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels. |
| [getClass()](#getClass--) |  |
| [getData()](#getData--) | Gets the data of the picture. |
| [getHeight()](#getHeight--) | Represents the height of shape, in unit of pixel. |
| [getHeightCM()](#getHeightCM--) | Represents the height of the shape, in unit of inches. |
| [getHeightInch()](#getHeightInch--) | Represents the height of the shape, in unit of inches. |
| [getHeightPt()](#getHeightPt--) | Represents the height of the shape, in unit of points. |
| [getHeightScale()](#getHeightScale--) | Gets the height scale,in unit of percent of the original picture height. |
| [getHtmlText()](#getHtmlText--) | Gets the html string which contains data and some formattings in this textbox. |
| [getHyperlink()](#getHyperlink--) | Gets the hyperlink of the shape. |
| [getID()](#getID--) | Gets /Sets the ID of the picture. |
| [getImageFormat()](#getImageFormat--) | Gets the image format of the picture. |
| [getLeft()](#getLeft--) | Represents the horizontal offset of shape from its left column, in unit of pixels. |
| [getLeftCM()](#getLeftCM--) | Represents the horizontal offset of shape from its left column, in unit of centimeters. |
| [getLeftInch()](#getLeftInch--) | Represents the horizontal offset of shape from its left column, in unit of inches. |
| [getLeftToCorner()](#getLeftToCorner--) | Represents the horizontal offset of shape from worksheet left board, in unit of pixels. |
| [getLinkedCell()](#getLinkedCell--) | Gets the worksheet range linked to the control's value. |
| [getLowerDeltaX()](#getLowerDeltaX--) | Gets the shape's horizontal offset from its lower right corner column. |
| [getLowerDeltaY()](#getLowerDeltaY--) | Gets the shape's vertical offset from its lower right corner row. |
| [getLowerRightColumn()](#getLowerRightColumn--) | Represents lower right corner column index. |
| [getLowerRightRow()](#getLowerRightRow--) | Represents lower right corner row index. |
| [getName()](#getName--) | Gets the name of the shape. |
| [getOriginalHeight()](#getOriginalHeight--) | Gets the original height of the picture. |
| [getOriginalHeightCM()](#getOriginalHeightCM--) | Gets the original height of picture, in unit of centimeters. |
| [getOriginalHeightInch()](#getOriginalHeightInch--) | Gets the original height of picture, in unit of inches. |
| [getOriginalWidth()](#getOriginalWidth--) | Gets the original width of the picture. |
| [getOriginalWidthCM()](#getOriginalWidthCM--) | Gets the original width of picture, in unit of centimeters. |
| [getOriginalWidthInch()](#getOriginalWidthInch--) | Gets the original width of picture, in unit of inches. |
| [getRelativeToOriginalPictureSize()](#getRelativeToOriginalPictureSize--) | Indicates whether shape is relative to original picture size. |
| [getRight()](#getRight--) | Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels. |
| [getRotationAngle()](#getRotationAngle--) | Gets the rotation of the shape. |
| [getSourceFullName()](#getSourceFullName--) | Gets the path and name of the source file for the linked image. |
| [getText()](#getText--) | Represents the string in this TextBox object. |
| [getTitle()](#getTitle--) | Specifies the title (caption) of the current shape object. |
| [getTop()](#getTop--) | Represents the vertical offset of shape from its top row, in unit of pixels. |
| [getTopCM()](#getTopCM--) | Represents the vertical offset of shape from its top row, in unit of centimeters. |
| [getTopInch()](#getTopInch--) | Represents the vertical offset of shape from its top row, in unit of inches. |
| [getTopToCorner()](#getTopToCorner--) | Represents the vertical offset of shape from worksheet top board, in unit of pixels. |
| [getUpperDeltaX()](#getUpperDeltaX--) | Gets the shape's horizontal offset from its upper left corner column. |
| [getUpperDeltaY()](#getUpperDeltaY--) | Gets the shape's vertical offset from its upper left corner row. |
| [getUpperLeftColumn()](#getUpperLeftColumn--) | Represents upper left corner column index. |
| [getUpperLeftRow()](#getUpperLeftRow--) | Represents upper left corner row index. |
| [getWidth()](#getWidth--) | Represents the width of shape, in unit of pixels. |
| [getWidthCM()](#getWidthCM--) | Represents the width of the shape, in unit of centimeters. |
| [getWidthInch()](#getWidthInch--) | Represents the width of the shape, in unit of inch. |
| [getWidthPt()](#getWidthPt--) | Represents the width of the shape, in unit of point. |
| [getWidthScale()](#getWidthScale--) | Gets the width scale, in unit of percent of the original picture width. |
| [getX()](#getX--) | Gets the horizonal offset of shape from worksheet left border,in unit of pixels. |
| [getY()](#getY--) | Gets the vertical offset of shape from worksheet top border,in unit of pixels. |
| [getZOrderPosition()](#getZOrderPosition--) | Returns the position of a shape in the z-order. |
| [hasLine()](#hasLine--) | Gets the line border of the shape is visible. |
| [hashCode()](#hashCode--) |  |
| [isFlippedVertically()](#isFlippedVertically--) | Gets whether shape is vertically flipped . |
| [isGroup()](#isGroup--) | Indicates whether the shape is a group. |
| [isHidden()](#isHidden--) | Indicates whether the object is visible. |
| [isLockAspectRatio()](#isLockAspectRatio--) | True means that don't allow changes in aspect ratio. |
| [isLocked()](#isLocked--) | True if the object is locked, False if the object can be modified when the sheet is protected. |
| [isTextWrapped()](#isTextWrapped--) | Gets the text wrapped type of the shape which contains text. |
| [move(int upperLeftRow, int upperLeftColumn)](#move-int-int-) | Moves the picture to a specified location. |
| [moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)](#moveToRange-int-int-int-int-) | Moves the shape to a specified range. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeHyperlink()](#removeHyperlink--) | Remove the hyperlink of the shape. |
| [saveToImage(InputStream s)](#saveToImage-java.io.InputStream-) | Creates the image and saves it to a stream . |
| [setAlternativeText(String value)](#setAlternativeText-java.lang.String-) | Returns or sets the descriptive (alternative) text string of the [GridShape](../../com.aspose.gridweb/gridshape) object. |
| [setBorderLineColor(Color value)](#setBorderLineColor-com.aspose.gridweb.Color-) | Represents the [Color](../../com.aspose.cells/color) of the border line of a picture. |
| [setBorderWeight(double value)](#setBorderWeight-double-) | Sets the weight of the border line of a picture in units of pt. |
| [setBottom(int value)](#setBottom-int-) | Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels. |
| [setData(byte[] value)](#setData-byte---) | Gets the data of the picture. |
| [setFlippedVertically(boolean value)](#setFlippedVertically-boolean-) | Sets whether shape is vertically flipped . |
| [setHasLine(boolean value)](#setHasLine-boolean-) | Sets the line border of the shape is visible. |
| [setHeight(int value)](#setHeight-int-) | Represents the height of shape, in unit of pixel. |
| [setHeightCM(double value)](#setHeightCM-double-) | Represents the height of the shape, in unit of inches. |
| [setHeightInch(double value)](#setHeightInch-double-) | Represents the height of the shape, in unit of inches. |
| [setHeightPt(double value)](#setHeightPt-double-) | Represents the height of the shape, in unit of points. |
| [setHeightScale(int value)](#setHeightScale-int-) | Sets the height scale,in unit of percent of the original picture height. |
| [setHidden(boolean value)](#setHidden-boolean-) | Indicates whether the object is visible. |
| [setHtmlText(String value)](#setHtmlText-java.lang.String-) | Sets the html string which contains data and some formattings in this textbox. |
| [setID(String value)](#setID-java.lang.String-) | Gets /Sets the ID of the picture. |
| [setLeft(int value)](#setLeft-int-) | Represents the horizontal offset of shape from its left column, in unit of pixels. |
| [setLeftCM(double value)](#setLeftCM-double-) | Represents the horizontal offset of shape from its left column, in unit of centimeters. |
| [setLeftInch(double value)](#setLeftInch-double-) | Represents the horizontal offset of shape from its left column, in unit of inches. |
| [setLeftToCorner(int value)](#setLeftToCorner-int-) | Represents the horizontal offset of shape from worksheet left board, in unit of pixels. |
| [setLinkedCell(String value)](#setLinkedCell-java.lang.String-) | Sets the worksheet range linked to the control's value. |
| [setLockAspectRatio(boolean value)](#setLockAspectRatio-boolean-) | True means that don't allow changes in aspect ratio. |
| [setLocked(boolean value)](#setLocked-boolean-) | True if the object is locked, False if the object can be modified when the sheet is protected. |
| [setLowerDeltaX(int value)](#setLowerDeltaX-int-) | Sets the shape's horizontal offset from its lower right corner column. |
| [setLowerDeltaY(int value)](#setLowerDeltaY-int-) | Sets the shape's vertical offset from its lower right corner row. |
| [setLowerRightColumn(int value)](#setLowerRightColumn-int-) | Represents lower right corner column index. |
| [setLowerRightRow(int value)](#setLowerRightRow-int-) | Represents lower right corner row index. |
| [setName(String value)](#setName-java.lang.String-) | Sets the name of the shape. |
| [setRelativeToOriginalPictureSize(boolean value)](#setRelativeToOriginalPictureSize-boolean-) | Indicates whether shape is relative to original picture size. |
| [setRight(int value)](#setRight-int-) | Represents the width of the shape's horizontal offset from its lower right corner column, in unit of pixels. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Sets the rotation of the shape. |
| [setSourceFullName(String value)](#setSourceFullName-java.lang.String-) | Sets the path and name of the source file for the linked image. |
| [setText(String value)](#setText-java.lang.String-) | Represents the string in this TextBox object. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Sets the text wrapped type of the shape which contains text. |
| [setTitle(String value)](#setTitle-java.lang.String-) | Specifies the title (caption) of the current shape object. |
| [setTop(int value)](#setTop-int-) | Represents the vertical offset of shape from its top row, in unit of pixels. |
| [setTopCM(double value)](#setTopCM-double-) | Represents the vertical offset of shape from its top row, in unit of centimeters. |
| [setTopInch(double value)](#setTopInch-double-) | Represents the vertical offset of shape from its top row, in unit of inches. |
| [setTopToCorner(int value)](#setTopToCorner-int-) | Represents the vertical offset of shape from worksheet top board, in unit of pixels. |
| [setUpperDeltaX(int value)](#setUpperDeltaX-int-) | Sets the shape's horizontal offset from its upper left corner column. |
| [setUpperDeltaY(int value)](#setUpperDeltaY-int-) | Sets the shape's vertical offset from its upper left corner row. |
| [setUpperLeftColumn(int value)](#setUpperLeftColumn-int-) | Represents upper left corner column index. |
| [setUpperLeftRow(int value)](#setUpperLeftRow-int-) | Represents upper left corner row index. |
| [setWidth(int value)](#setWidth-int-) | Represents the width of shape, in unit of pixels. |
| [setWidthCM(double value)](#setWidthCM-double-) | Represents the width of the shape, in unit of centimeters. |
| [setWidthInch(double value)](#setWidthInch-double-) | Represents the width of the shape, in unit of inch. |
| [setWidthPt(double value)](#setWidthPt-double-) | Represents the width of the shape, in unit of point. |
| [setWidthScale(int value)](#setWidthScale-int-) | Sets the width scale, in unit of percent of the original picture width. |
| [setX(int value)](#setX-int-) | Sets the horizonal offset of shape from worksheet left border,in unit of pixels. |
| [setY(int value)](#setY-int-) | Sets the vertical offset of shape from worksheet top border,in unit of pixels. |
| [setZOrderPosition(int value)](#setZOrderPosition-int-) | Returns the position of a shape in the z-order. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addHyperlink(String address) {#addHyperlink-java.lang.String-}
```
public GridHyperlink addHyperlink(String address)
```
Adds a hyperlink to the shape.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| address | java.lang.String | Address of the hyperlink. |
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
Returns or sets the descriptive (alternative) text string of the [GridShape](../../com.aspose.gridweb/gridshape) object.
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
Gets the weight of the border line of a picture in units of pt.
**Returns:**
double
### getBottom() {#getBottom--}
```
public int getBottom()
```
Represents the width of the shape's vertical offset from its lower bottom corner row, in unit of pixels.
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
Gets the height scale,in unit of percent of the original picture height. If the shape is not picture ,the HeightScale property only returns 100;
**Returns:**
int
### getHtmlText() {#getHtmlText--}
```
public String getHtmlText()
```
Gets the html string which contains data and some formattings in this textbox.
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
Gets /Sets the ID of the picture.
**Returns:**
java.lang.String
### getImageFormat() {#getImageFormat--}
```
public int getImageFormat()
```
Gets the image format of the picture.
See [GridImageType](../../com.aspose.gridweb/gridimagetype).
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
### getLeftToCorner() {#getLeftToCorner--}
```
public int getLeftToCorner()
```
Represents the horizontal offset of shape from worksheet left board, in unit of pixels.
**Returns:**
int
### getLinkedCell() {#getLinkedCell--}
```
public String getLinkedCell()
```
Gets the worksheet range linked to the control's value.
**Returns:**
java.lang.String
### getLowerDeltaX() {#getLowerDeltaX--}
```
public int getLowerDeltaX()
```
Gets the shape's horizontal offset from its lower right corner column. The range of value is 0 to 1024.
**Returns:**
int
### getLowerDeltaY() {#getLowerDeltaY--}
```
public int getLowerDeltaY()
```
Gets the shape's vertical offset from its lower right corner row. The range of value is 0 to 256.
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
Gets the name of the shape.
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
Gets the rotation of the shape.
**Returns:**
double
### getSourceFullName() {#getSourceFullName--}
```
public String getSourceFullName()
```
Gets the path and name of the source file for the linked image.
**Remarks**
The default value is an empty string. If SourceFullName is not an empty string, the image is linked. If SourceFullName is not an empty string, but Data is null, then the image is linked and not stored in the file.
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
Specifies the title (caption) of the current shape object.
**Returns:**
java.lang.String
### getTop() {#getTop--}
```
public int getTop()
```
Represents the vertical offset of shape from its top row, in unit of pixels.
**Remarks**
If the shape is in the chart, represents the vertical offset of shape from its top border.
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
### getTopToCorner() {#getTopToCorner--}
```
public int getTopToCorner()
```
Represents the vertical offset of shape from worksheet top board, in unit of pixels.
**Returns:**
int
### getUpperDeltaX() {#getUpperDeltaX--}
```
public int getUpperDeltaX()
```
Gets the shape's horizontal offset from its upper left corner column. The range of value is 0 to 1024.
**Returns:**
int
### getUpperDeltaY() {#getUpperDeltaY--}
```
public int getUpperDeltaY()
```
Gets the shape's vertical offset from its upper left corner row. The range of value is 0 to 256.
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
Represents upper left corner row index.
**Remarks**
If the shape is in the shape or in the group , UpperLeftRow will be ignored.
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
Gets the width scale, in unit of percent of the original picture width. If the shape is not picture ,the WidthScale property only returns 100;
**Returns:**
int
### getX() {#getX--}
```
public int getX()
```
Gets the horizonal offset of shape from worksheet left border,in unit of pixels.
**Returns:**
int
### getY() {#getY--}
```
public int getY()
```
Gets the vertical offset of shape from worksheet top border,in unit of pixels.
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
Gets the line border of the shape is visible.
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
Gets whether shape is vertically flipped .
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
Gets the text wrapped type of the shape which contains text.
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
### moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn) {#moveToRange-int-int-int-int-}
```
public void moveToRange(int upperLeftRow, int upperLeftColumn, int lowerRightRow, int lowerRightColumn)
```
Moves the shape to a specified range.
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
Returns or sets the descriptive (alternative) text string of the [GridShape](../../com.aspose.gridweb/gridshape) object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setBorderLineColor(Color value) {#setBorderLineColor-com.aspose.gridweb.Color-}
```
public void setBorderLineColor(Color value)
```
Represents the [Color](../../com.aspose.cells/color) of the border line of a picture.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |
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
### setData(byte[] value) {#setData-byte---}
```
public void setData(byte[] value)
```
Gets the data of the picture.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | byte[] |  |
### setFlippedVertically(boolean value) {#setFlippedVertically-boolean-}
```
public void setFlippedVertically(boolean value)
```
Sets whether shape is vertically flipped .
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
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
Represents the height of the shape, in unit of inches.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
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
Sets the html string which contains data and some formattings in this textbox.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setID(String value) {#setID-java.lang.String-}
```
public void setID(String value)
```
Gets /Sets the ID of the picture.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
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
Represents the horizontal offset of shape from worksheet left board, in unit of pixels.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setLinkedCell(String value) {#setLinkedCell-java.lang.String-}
```
public void setLinkedCell(String value)
```
Sets the worksheet range linked to the control's value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
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
### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```
Sets the name of the shape.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
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
### setSourceFullName(String value) {#setSourceFullName-java.lang.String-}
```
public void setSourceFullName(String value)
```
Sets the path and name of the source file for the linked image.
**Remarks**
The default value is an empty string. If SourceFullName is not an empty string, the image is linked. If SourceFullName is not an empty string, but Data is null, then the image is linked and not stored in the file.
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
Represents the vertical offset of shape from its top row, in unit of pixels.
**Remarks**
If the shape is in the chart, represents the vertical offset of shape from its top border.
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
Represents the vertical offset of shape from worksheet top board, in unit of pixels.
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
Represents upper left corner row index.
**Remarks**
If the shape is in the shape or in the group , UpperLeftRow will be ignored.
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
Sets the horizonal offset of shape from worksheet left border,in unit of pixels.
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
