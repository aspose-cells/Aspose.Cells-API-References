##DataBar
Describe the DataBar conditional formatting rule.
**Inheritance:**
java.lang.Object
```
public class DataBar
```
Describe the DataBar conditional formatting rule. This conditional formatting rule displays a gradated data bar in the range of cells.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
Worksheet sheet = workbook.getWorksheets().get(0);
//Adds an empty conditional formatting
int index = sheet.getConditionalFormattings().add();
FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
//Sets the conditional format range.
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 2;
ca.StartColumn = 0;
ca.EndColumn = 0;
fcs.addArea(ca);
//Adds condition.
int idx = fcs.addCondition(FormatConditionType.DATA_BAR);
fcs.addArea(ca);
FormatCondition cond = fcs.get(idx);
//Get Databar
DataBar dataBar = cond.getDataBar();
dataBar.setColor(Color.getOrange());
//Set Databar properties
dataBar.getMinCfvo().setType(FormatConditionValueType.PERCENTILE);
dataBar.getMinCfvo().setValue(30);
dataBar.setShowValue(false);
dataBar.getBarBorder().setType(DataBarBorderType.SOLID);
dataBar.getBarBorder().setColor(Color.getPlum());
dataBar.setBarFillType(DataBarFillType.SOLID);
dataBar.setAxisColor(Color.getRed());
dataBar.setAxisPosition(DataBarAxisPosition.MIDPOINT);
dataBar.getNegativeBarFormat().setColorType(DataBarNegativeColorType.COLOR);
dataBar.getNegativeBarFormat().setColor(Color.getWhite());
dataBar.getNegativeBarFormat().setBorderColorType(DataBarNegativeColorType.COLOR);
dataBar.getNegativeBarFormat().setBorderColor(Color.getYellow());
//Put Cell Values
Cell cell1 = sheet.getCells().get("A1");
cell1.putValue(10);
Cell cell2 = sheet.getCells().get("A2");
cell2.putValue(120);
Cell cell3 = sheet.getCells().get("A3");
cell3.putValue(260);
//Saving the Excel file
workbook.save("book1.xlsx");
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAxisColor()](#getAxisColor--) | Gets the color of the axis for cells with conditional formatting as data bars. |
| [getAxisPosition()](#getAxisPosition--) | Gets the position of the axis of the data bars specified by a conditional formatting rule. |
| [getBarBorder()](#getBarBorder--) | Gets an object that specifies the border of a data bar. |
| [getBarFillType()](#getBarFillType--) | Gets how a data bar is filled with color. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Gets this DataBar's Color. |
| [getDirection()](#getDirection--) | Gets the direction the databar is displayed. |
| [getMaxCfvo()](#getMaxCfvo--) | Gets this DataBar's max value object. |
| [getMaxLength()](#getMaxLength--) | Represents the max length of data bar . |
| [getMinCfvo()](#getMinCfvo--) | Gets this DataBar's min value object. |
| [getMinLength()](#getMinLength--) | Represents the min length of data bar . |
| [getNegativeBarFormat()](#getNegativeBarFormat--) | Gets the NegativeBarFormat object associated with a data bar conditional formatting rule. |
| [getShowValue()](#getShowValue--) | Gets the flag indicating whether to show the values of the cells on which this data bar is applied. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAxisColor(Color value)](#setAxisColor-com.aspose.cells.Color-) | Gets the color of the axis for cells with conditional formatting as data bars. |
| [setAxisPosition(int value)](#setAxisPosition-int-) | Sets the position of the axis of the data bars specified by a conditional formatting rule. |
| [setBarFillType(int value)](#setBarFillType-int-) | Sets how a data bar is filled with color. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | Sets this DataBar's Color. |
| [setDirection(int value)](#setDirection-int-) | Sets the direction the databar is displayed. |
| [setMaxLength(int value)](#setMaxLength-int-) | Represents the max length of data bar . |
| [setMinLength(int value)](#setMinLength-int-) | Represents the min length of data bar . |
| [setShowValue(boolean value)](#setShowValue-boolean-) | Sets the flag indicating whether to show the values of the cells on which this data bar is applied. |
| [toImage(Cell cell, ImageOrPrintOptions imgOpts)](#toImage-com.aspose.cells.Cell-com.aspose.cells.ImageOrPrintOptions-) | Render data bar in cell to image byte array. |
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
### getAxisColor() {#getAxisColor--}
```
public Color getAxisColor()
```
Gets the color of the axis for cells with conditional formatting as data bars.
**Returns:**
[Color](../../com.aspose.cells/color)
### getAxisPosition() {#getAxisPosition--}
```
public int getAxisPosition()
```
Gets the position of the axis of the data bars specified by a conditional formatting rule.
See [DataBarAxisPosition](../../com.aspose.cells/databaraxisposition).
**Returns:**
int
### getBarBorder() {#getBarBorder--}
```
public DataBarBorder getBarBorder()
```
Gets an object that specifies the border of a data bar.
**Returns:**
[DataBarBorder](../../com.aspose.cells/databarborder)
### getBarFillType() {#getBarFillType--}
```
public int getBarFillType()
```
Gets how a data bar is filled with color.
See [DataBarFillType](../../com.aspose.cells/databarfilltype).
**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getColor() {#getColor--}
```
public Color getColor()
```
Gets this DataBar's Color.
**Returns:**
[Color](../../com.aspose.cells/color)
### getDirection() {#getDirection--}
```
public int getDirection()
```
Gets the direction the databar is displayed.
See [TextDirectionType](../../com.aspose.cells/textdirectiontype).
**Returns:**
int
### getMaxCfvo() {#getMaxCfvo--}
```
public ConditionalFormattingValue getMaxCfvo()
```
Gets this DataBar's max value object. Cannot set null or CFValueObject with type FormatConditionValueType.Min to it.
**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMaxLength() {#getMaxLength--}
```
public int getMaxLength()
```
Represents the max length of data bar .
**Returns:**
int
### getMinCfvo() {#getMinCfvo--}
```
public ConditionalFormattingValue getMinCfvo()
```
Gets this DataBar's min value object. Cannot set null or CFValueObject with type FormatConditionValueType.Max to it.
**Returns:**
[ConditionalFormattingValue](../../com.aspose.cells/conditionalformattingvalue)
### getMinLength() {#getMinLength--}
```
public int getMinLength()
```
Represents the min length of data bar .
**Returns:**
int
### getNegativeBarFormat() {#getNegativeBarFormat--}
```
public NegativeBarFormat getNegativeBarFormat()
```
Gets the NegativeBarFormat object associated with a data bar conditional formatting rule.
**Returns:**
[NegativeBarFormat](../../com.aspose.cells/negativebarformat)
### getShowValue() {#getShowValue--}
```
public boolean getShowValue()
```
Gets the flag indicating whether to show the values of the cells on which this data bar is applied. Default value is true.
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
### setAxisColor(Color value) {#setAxisColor-com.aspose.cells.Color-}
```
public void setAxisColor(Color value)
```
Gets the color of the axis for cells with conditional formatting as data bars.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |
### setAxisPosition(int value) {#setAxisPosition-int-}
```
public void setAxisPosition(int value)
```
Sets the position of the axis of the data bars specified by a conditional formatting rule.
See [DataBarAxisPosition](../../com.aspose.cells/databaraxisposition).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setBarFillType(int value) {#setBarFillType-int-}
```
public void setBarFillType(int value)
```
Sets how a data bar is filled with color.
See [DataBarFillType](../../com.aspose.cells/databarfilltype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```
Sets this DataBar's Color.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |
### setDirection(int value) {#setDirection-int-}
```
public void setDirection(int value)
```
Sets the direction the databar is displayed.
See [TextDirectionType](../../com.aspose.cells/textdirectiontype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setMaxLength(int value) {#setMaxLength-int-}
```
public void setMaxLength(int value)
```
Represents the max length of data bar .
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setMinLength(int value) {#setMinLength-int-}
```
public void setMinLength(int value)
```
Represents the min length of data bar .
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setShowValue(boolean value) {#setShowValue-boolean-}
```
public void setShowValue(boolean value)
```
Sets the flag indicating whether to show the values of the cells on which this data bar is applied. Default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### toImage(Cell cell, ImageOrPrintOptions imgOpts) {#toImage-com.aspose.cells.Cell-com.aspose.cells.ImageOrPrintOptions-}
```
public byte[] toImage(Cell cell, ImageOrPrintOptions imgOpts)
```
Render data bar in cell to image byte array.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Indicate the data bar in which cell to be rendered |
| imgOpts | [ImageOrPrintOptions](../../com.aspose.cells/imageorprintoptions) | ImageOrPrintOptions contains some property of output image |
**Returns:**
byte[] -
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
