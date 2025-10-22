##TextBoxOptions
Represents the text options of the shape
**Inheritance:**
java.lang.Object
```
public class TextBoxOptions
```
Represents the text options of the shape
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
int index = workbook.getWorksheets().get(0).getTextBoxes().add(0, 0, 350, 350);
Shape shape = workbook.getWorksheets().get(0).getTextBoxes().get(index);
shape.setText("This is test.");
//do your business
//Save the excel file.
workbook.save("exmaple.xlsx");
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowTextToOverflow()](#getAllowTextToOverflow--) | Whether allow text to overflow shape. |
| [getBottomMarginPt()](#getBottomMarginPt--) | Returns the bottom margin in unit of Points |
| [getClass()](#getClass--) |  |
| [getLeftMarginPt()](#getLeftMarginPt--) | Gets the left margin in unit of Points. |
| [getResizeToFitText()](#getResizeToFitText--) | Indicates whether to resize the shape to fit the text |
| [getRightMarginPt()](#getRightMarginPt--) | Gets the right margin in unit of Points. |
| [getShapeTextDirection()](#getShapeTextDirection--) | Gets the text display direction within a given text body. |
| [getShapeTextVerticalAlignment()](#getShapeTextVerticalAlignment--) | It corresponds to "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel. |
| [getTopMarginPt()](#getTopMarginPt--) | Gets the top margin in unit of Points. |
| [getWrapTextInShape()](#getWrapTextInShape--) | Specifies text wrapping within a shape. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowTextToOverflow(boolean value)](#setAllowTextToOverflow-boolean-) | Whether allow text to overflow shape. |
| [setBottomMarginPt(double value)](#setBottomMarginPt-double-) | Returns the bottom margin in unit of Points |
| [setLeftMarginPt(double value)](#setLeftMarginPt-double-) | Sets the left margin in unit of Points. |
| [setResizeToFitText(boolean value)](#setResizeToFitText-boolean-) | Indicates whether to resize the shape to fit the text |
| [setRightMarginPt(double value)](#setRightMarginPt-double-) | Sets the right margin in unit of Points. |
| [setShapeTextDirection(int value)](#setShapeTextDirection-int-) | Sets the text display direction within a given text body. |
| [setShapeTextVerticalAlignment(int value)](#setShapeTextVerticalAlignment-int-) | It corresponds to "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel. |
| [setTopMarginPt(double value)](#setTopMarginPt-double-) | Sets the top margin in unit of Points. |
| [setWrapTextInShape(boolean value)](#setWrapTextInShape-boolean-) | Specifies text wrapping within a shape. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getAllowTextToOverflow() {#getAllowTextToOverflow--}
```
public boolean getAllowTextToOverflow()
```
Whether allow text to overflow shape.
**Example**
```
shape.getTextBoxOptions().setAllowTextToOverflow(true);
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
shape.getTextBoxOptions().setBottomMarginPt(0.2d);
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
Gets the left margin in unit of Points.
**Example**
```
shape.getTextBoxOptions().setLeftMarginPt(0.2d);
```
**Returns:**
double
### getResizeToFitText() {#getResizeToFitText--}
```
public boolean getResizeToFitText()
```
Indicates whether to resize the shape to fit the text
**Example**
```
shape.getTextBoxOptions().setResizeToFitText(true);
```
**Returns:**
boolean
### getRightMarginPt() {#getRightMarginPt--}
```
public double getRightMarginPt()
```
Gets the right margin in unit of Points.
**Example**
```
shape.getTextBoxOptions().setRightMarginPt(0.2d);
```
**Returns:**
double
### getShapeTextDirection() {#getShapeTextDirection--}
```
public int getShapeTextDirection()
```
Gets the text display direction within a given text body. It corresponds to "Format Shape - Text Options - Text Box - Text direction" in Excel
See [TextVerticalType](../../com.aspose.cells/textverticaltype).
**Example**
```
shape.getTextBoxOptions().setShapeTextDirection(TextVerticalType.VERTICAL);
```
**Returns:**
int
### getShapeTextVerticalAlignment() {#getShapeTextVerticalAlignment--}
```
public int getShapeTextVerticalAlignment()
```
It corresponds to "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel.
See [ShapeTextVerticalAlignmentType](../../com.aspose.cells/shapetextverticalalignmenttype).
**Example**
```
shape.getTextBoxOptions().setShapeTextVerticalAlignment(ShapeTextVerticalAlignmentType.LEFT);
```
**Returns:**
int
### getTopMarginPt() {#getTopMarginPt--}
```
public double getTopMarginPt()
```
Gets the top margin in unit of Points.
**Example**
```
shape.getTextBoxOptions().setTopMarginPt(0.2d);
```
**Returns:**
double
### getWrapTextInShape() {#getWrapTextInShape--}
```
public boolean getWrapTextInShape()
```
Specifies text wrapping within a shape. False - No wrapping will occur on text body. True - Wrapping will occur on text body.
**Example**
```
shape.getTextBoxOptions().setWrapTextInShape(true);
```
**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### setAllowTextToOverflow(boolean value) {#setAllowTextToOverflow-boolean-}
```
public void setAllowTextToOverflow(boolean value)
```
Whether allow text to overflow shape.
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
Sets the left margin in unit of Points.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setResizeToFitText(boolean value) {#setResizeToFitText-boolean-}
```
public void setResizeToFitText(boolean value)
```
Indicates whether to resize the shape to fit the text
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setRightMarginPt(double value) {#setRightMarginPt-double-}
```
public void setRightMarginPt(double value)
```
Sets the right margin in unit of Points.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setShapeTextDirection(int value) {#setShapeTextDirection-int-}
```
public void setShapeTextDirection(int value)
```
Sets the text display direction within a given text body. It corresponds to "Format Shape - Text Options - Text Box - Text direction" in Excel
See [TextVerticalType](../../com.aspose.cells/textverticaltype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setShapeTextVerticalAlignment(int value) {#setShapeTextVerticalAlignment-int-}
```
public void setShapeTextVerticalAlignment(int value)
```
It corresponds to "Format Shape - Text Options - Text Box - Vertical Alignment" in Excel.
See [ShapeTextVerticalAlignmentType](../../com.aspose.cells/shapetextverticalalignmenttype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setTopMarginPt(double value) {#setTopMarginPt-double-}
```
public void setTopMarginPt(double value)
```
Sets the top margin in unit of Points.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setWrapTextInShape(boolean value) {#setWrapTextInShape-boolean-}
```
public void setWrapTextInShape(boolean value)
```
Specifies text wrapping within a shape. False - No wrapping will occur on text body. True - Wrapping will occur on text body.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
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
