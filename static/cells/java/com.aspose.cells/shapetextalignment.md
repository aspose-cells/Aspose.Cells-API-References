##ShapeTextAlignment
Represents the setting of shapes text alignment
**Inheritance:**
java.lang.Object
```
public class ShapeTextAlignment
```
Represents the setting of shape's text alignment;
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
Shape shape = workbook.getWorksheets().get(0).getShapes().addRectangle(1, 0, 1, 0, 50, 100);
ShapeTextAlignment shapeTextAlignment = shape.getTextBody().getTextAlignment();
//do your business
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | Determines whether this instance has the same value as another specified [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) object. |
| [getAutoSize()](#getAutoSize--) | Indicates if size of shape is adjusted automatically according to its content. |
| [getBottomMarginPt()](#getBottomMarginPt--) | Returns the bottom margin in unit of Points |
| [getClass()](#getClass--) |  |
| [getLeftMarginPt()](#getLeftMarginPt--) | Returns the left margin in unit of Points |
| [getNumberOfColumns()](#getNumberOfColumns--) | Gets the number of columns of text in the bounding rectangle. |
| [getRightMarginPt()](#getRightMarginPt--) | Returns the right margin in unit of Points |
| [getRotateTextWithShape()](#getRotateTextWithShape--) | Indicates whether rotating text with shape. |
| [getRotationAngle()](#getRotationAngle--) | Gets the rotation of the shape. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | Gets the text horizontal overflow type of the text box. |
| [getTextShapeType()](#getTextShapeType--) | Gets the transform type of text. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | Gets the text vertical overflow type of the text box. |
| [getTextVerticalType()](#getTextVerticalType--) | Gets the text direction. |
| [getTopMarginPt()](#getTopMarginPt--) | Returns the top margin in unit of Points |
| [hashCode()](#hashCode--) |  |
| [isAutoMargin()](#isAutoMargin--) | Indicates whether the margin of the text frame is automatic. |
| [isLockedText()](#isLockedText--) | Indicates whether the shape is locked when worksheet is protected. |
| [isTextWrapped()](#isTextWrapped--) | Gets the text wrapped type of the shape which contains text. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoMargin(boolean value)](#setAutoMargin-boolean-) | Indicates whether the margin of the text frame is automatic. |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | Indicates if size of shape is adjusted automatically according to its content. |
| [setBottomMarginPt(double value)](#setBottomMarginPt-double-) | Returns the bottom margin in unit of Points |
| [setLeftMarginPt(double value)](#setLeftMarginPt-double-) | Returns the left margin in unit of Points |
| [setLockedText(boolean value)](#setLockedText-boolean-) | Indicates whether the shape is locked when worksheet is protected. |
| [setNumberOfColumns(int value)](#setNumberOfColumns-int-) | Sets the number of columns of text in the bounding rectangle. |
| [setRightMarginPt(double value)](#setRightMarginPt-double-) | Returns the right margin in unit of Points |
| [setRotateTextWithShape(boolean value)](#setRotateTextWithShape-boolean-) | Indicates whether rotating text with shape. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | Sets the rotation of the shape. |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | Sets the text horizontal overflow type of the text box. |
| [setTextShapeType(int value)](#setTextShapeType-int-) | Sets the transform type of text. |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | Sets the text vertical overflow type of the text box. |
| [setTextVerticalType(int value)](#setTextVerticalType-int-) | Sets the text direction. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | Sets the text wrapped type of the shape which contains text. |
| [setTopMarginPt(double value)](#setTopMarginPt-double-) | Returns the top margin in unit of Points |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```
Determines whether this instance has the same value as another specified [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) object.
**Example**
```
//You have to make sure that the index value in this line of code exists
ShapeTextAlignment obj = workbook.getWorksheets().get(0).getShapes().get(0).getTextBody().getTextAlignment();
if (shapeTextAlignment.equals(obj))
{
//do what you want
}
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | The [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) object to compare with this instance. |
**Returns:**
boolean - true if the value of the obj parameter is the same as the value of this instance; otherwise, false. If obj is null, this method returns false.
### getAutoSize() {#getAutoSize--}
```
public boolean getAutoSize()
```
Indicates if size of shape is adjusted automatically according to its content.
**Example**
```
shapeTextAlignment.setAutoSize(false);
```
**Returns:**
boolean
### getBottomMarginPt() {#getBottomMarginPt--}
```
public double getBottomMarginPt()
```
Returns the bottom margin in unit of Points
**Example**
```
shapeTextAlignment.setBottomMarginPt(2.0d);
```
**Returns:**
double
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getLeftMarginPt() {#getLeftMarginPt--}
```
public double getLeftMarginPt()
```
Returns the left margin in unit of Points
**Example**
```
shapeTextAlignment.setLeftMarginPt(2.0d);
```
**Returns:**
double
### getNumberOfColumns() {#getNumberOfColumns--}
```
public int getNumberOfColumns()
```
Gets the number of columns of text in the bounding rectangle.
**Returns:**
int
### getRightMarginPt() {#getRightMarginPt--}
```
public double getRightMarginPt()
```
Returns the right margin in unit of Points
**Example**
```
shapeTextAlignment.setRightMarginPt(2.0d);
```
**Returns:**
double
### getRotateTextWithShape() {#getRotateTextWithShape--}
```
public boolean getRotateTextWithShape()
```
Indicates whether rotating text with shape.
**Example**
```
shapeTextAlignment.setRotateTextWithShape(true);
```
**Returns:**
boolean
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```
Gets the rotation of the shape.
**Example**
```
shapeTextAlignment.setRotationAngle(90);
```
**Returns:**
double
### getTextHorizontalOverflow() {#getTextHorizontalOverflow--}
```
public int getTextHorizontalOverflow()
```
Gets the text horizontal overflow type of the text box.
See [TextOverflowType](../../com.aspose.cells/textoverflowtype).
**Example**
```
shapeTextAlignment.setTextHorizontalOverflow(TextOverflowType.CLIP);
```
**Returns:**
int
### getTextShapeType() {#getTextShapeType--}
```
public int getTextShapeType()
```
Gets the transform type of text.
See [AutoShapeType](../../com.aspose.cells/autoshapetype).
**Example**
```
//Usually do not modify this value unless you know exactly what the modification will result in
shapeTextAlignment.setTextShapeType(AutoShapeType.TEXT_BOX);
```
**Returns:**
int
### getTextVerticalOverflow() {#getTextVerticalOverflow--}
```
public int getTextVerticalOverflow()
```
Gets the text vertical overflow type of the text box.
See [TextOverflowType](../../com.aspose.cells/textoverflowtype).
**Example**
```
shapeTextAlignment.setTextVerticalOverflow(TextOverflowType.CLIP);
```
**Returns:**
int
### getTextVerticalType() {#getTextVerticalType--}
```
public int getTextVerticalType()
```
Gets the text direction.
See [TextVerticalType](../../com.aspose.cells/textverticaltype).
**Example**
```
shapeTextAlignment.setTextVerticalType(com.aspose.cells.TextVerticalType.HORIZONTAL);
```
**Returns:**
int
### getTopMarginPt() {#getTopMarginPt--}
```
public double getTopMarginPt()
```
Returns the top margin in unit of Points
**Example**
```
shapeTextAlignment.setTopMarginPt(2.0d);
```
**Returns:**
double
### hashCode() {#hashCode--}
```
public int hashCode()
```
**Returns:**
int -
### isAutoMargin() {#isAutoMargin--}
```
public boolean isAutoMargin()
```
Indicates whether the margin of the text frame is automatic.
**Example**
```
shapeTextAlignment.setAutoMargin(true);
```
**Returns:**
boolean
### isLockedText() {#isLockedText--}
```
public boolean isLockedText()
```
Indicates whether the shape is locked when worksheet is protected.
**Remarks**
Only works when worksheet is protected.
**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```
Gets the text wrapped type of the shape which contains text.
**Example**
```
shapeTextAlignment.setTextWrapped(true);
```
**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### setAutoMargin(boolean value) {#setAutoMargin-boolean-}
```
public void setAutoMargin(boolean value)
```
Indicates whether the margin of the text frame is automatic.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```
Indicates if size of shape is adjusted automatically according to its content.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setBottomMarginPt(double value) {#setBottomMarginPt-double-}
```
public void setBottomMarginPt(double value)
```
Returns the bottom margin in unit of Points
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setLeftMarginPt(double value) {#setLeftMarginPt-double-}
```
public void setLeftMarginPt(double value)
```
Returns the left margin in unit of Points
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setLockedText(boolean value) {#setLockedText-boolean-}
```
public void setLockedText(boolean value)
```
Indicates whether the shape is locked when worksheet is protected.
**Remarks**
Only works when worksheet is protected.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setNumberOfColumns(int value) {#setNumberOfColumns-int-}
```
public void setNumberOfColumns(int value)
```
Sets the number of columns of text in the bounding rectangle.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setRightMarginPt(double value) {#setRightMarginPt-double-}
```
public void setRightMarginPt(double value)
```
Returns the right margin in unit of Points
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setRotateTextWithShape(boolean value) {#setRotateTextWithShape-boolean-}
```
public void setRotateTextWithShape(boolean value)
```
Indicates whether rotating text with shape.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```
Sets the rotation of the shape.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```
Sets the text horizontal overflow type of the text box.
See [TextOverflowType](../../com.aspose.cells/textoverflowtype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```
Sets the transform type of text.
See [AutoShapeType](../../com.aspose.cells/autoshapetype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```
Sets the text vertical overflow type of the text box.
See [TextOverflowType](../../com.aspose.cells/textoverflowtype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setTextVerticalType(int value) {#setTextVerticalType-int-}
```
public void setTextVerticalType(int value)
```
Sets the text direction.
See [TextVerticalType](../../com.aspose.cells/textverticaltype).
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
### setTopMarginPt(double value) {#setTopMarginPt-double-}
```
public void setTopMarginPt(double value)
```
Returns the top margin in unit of Points
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
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
