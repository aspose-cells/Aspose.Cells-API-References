##Name
Represents a defined name for a range of cells.
**Inheritance:**
java.lang.Object
```
public class Name
```
Represents a defined name for a range of cells.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Accessing the first worksheet in the Excel file
Worksheet worksheet = workbook.getWorksheets().get(0);
//Creating a named range
Range range = worksheet.getCells().createRange("B4", "G14");
//Setting the name of the named range
range.setName("TestRange");
//Saving the modified Excel file in default (that is Excel 2000) format
workbook.save("output.xls");
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getComment()](#getComment--) | Gets the comment of the name. |
| [getFullText()](#getFullText--) | Gets the name full text of the object with the scope setting. |
| [getR1C1RefersTo()](#getR1C1RefersTo--) | Gets a R1C1 reference of the [Name](../../com.aspose.cells/name). |
| [getRange()](#getRange--) | Gets the range if this name refers to a range. |
| [getRange(boolean recalculate)](#getRange-boolean-) | Gets the range if this name refers to a range |
| [getRange(int sheetIndex, int row, int column)](#getRange-int-int-int-) | Gets the range if this name refers to a range. |
| [getRanges()](#getRanges--) | Gets all ranges referred by this name. |
| [getRanges(boolean recalculate)](#getRanges-boolean-) | Gets all ranges referred by this name. |
| [getReferredAreas(boolean recalculate)](#getReferredAreas-boolean-) | Gets all references referred by this name. |
| [getRefersTo()](#getRefersTo--) | Returns or sets the formula that the name is defined to refer to, beginning with an equal sign. |
| [getRefersTo(boolean isR1C1, boolean isLocal)](#getRefersTo-boolean-boolean-) | Get the reference of this Name. |
| [getRefersTo(boolean isR1C1, boolean isLocal, int row, int column)](#getRefersTo-boolean-boolean-int-int-) | Get the reference of this Name based on specified cell. |
| [getSheetIndex()](#getSheetIndex--) | Indicates this name belongs to Workbook or Worksheet. 0 = Global name, otherwise index to sheet (one-based) |
| [getText()](#getText--) | Gets the name text of the object. |
| [hashCode()](#hashCode--) |  |
| [isReferred()](#isReferred--) | Indicates whether this name is referred by other formulas. |
| [isVisible()](#isVisible--) | Indicates whether the name is visible. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setComment(String value)](#setComment-java.lang.String-) | Sets the comment of the name. |
| [setR1C1RefersTo(String value)](#setR1C1RefersTo-java.lang.String-) | Sets a R1C1 reference of the [Name](../../com.aspose.cells/name). |
| [setRefersTo(String value)](#setRefersTo-java.lang.String-) | Returns or sets the formula that the name is defined to refer to, beginning with an equal sign. |
| [setRefersTo(String refersTo, boolean isR1C1, boolean isLocal)](#setRefersTo-java.lang.String-boolean-boolean-) | Set the reference of this Name. |
| [setSheetIndex(int value)](#setSheetIndex-int-) | Indicates this name belongs to Workbook or Worksheet. 0 = Global name, otherwise index to sheet (one-based) |
| [setText(String value)](#setText-java.lang.String-) | Gets the name text of the object. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indicates whether the name is visible. |
| [toString()](#toString--) | Returns a string represents the current Range object. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getComment() {#getComment--}
```
public String getComment()
```
Gets the comment of the name. Only applies for Excel 2007 or higher versions.
**Returns:**
java.lang.String
### getFullText() {#getFullText--}
```
public String getFullText()
```
Gets the name full text of the object with the scope setting.
**Returns:**
java.lang.String
### getR1C1RefersTo() {#getR1C1RefersTo--}
```
public String getR1C1RefersTo()
```
Gets a R1C1 reference of the [Name](../../com.aspose.cells/name).
**Returns:**
java.lang.String
### getRange() {#getRange--}
```
public Range getRange()
```
Gets the range if this name refers to a range.
**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRange(boolean recalculate) {#getRange-boolean-}
```
public Range getRange(boolean recalculate)
```
Gets the range if this name refers to a range
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | boolean | whether recalculate it if this name has been calculated before this invocation. |
**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRange(int sheetIndex, int row, int column) {#getRange-int-int-int-}
```
public Range getRange(int sheetIndex, int row, int column)
```
Gets the range if this name refers to a range. If the reference of this name is not absolute, the range may be different for different cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | int | The according sheet index. |
| row | int | The according row index. |
| column | int | The according column index |
**Returns:**
[Range](../../com.aspose.cells/range) - The range.
### getRanges() {#getRanges--}
```
public Range[] getRanges()
```
Gets all ranges referred by this name.
**Returns:**
com.aspose.cells.Range[] - All ranges.
### getRanges(boolean recalculate) {#getRanges-boolean-}
```
public Range[] getRanges(boolean recalculate)
```
Gets all ranges referred by this name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | boolean | whether recalculate it if this name has been calculated before this invocation. |
**Returns:**
com.aspose.cells.Range[] - All ranges.
### getReferredAreas(boolean recalculate) {#getReferredAreas-boolean-}
```
public ReferredArea[] getReferredAreas(boolean recalculate)
```
Gets all references referred by this name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| recalculate | boolean | whether recalculate it if this name has been calculated before this invocation. |
**Returns:**
com.aspose.cells.ReferredArea[] - All ranges.
### getRefersTo() {#getRefersTo--}
```
public String getRefersTo()
```
Returns or sets the formula that the name is defined to refer to, beginning with an equal sign.
**Returns:**
java.lang.String
### getRefersTo(boolean isR1C1, boolean isLocal) {#getRefersTo-boolean-boolean-}
```
public String getRefersTo(boolean isR1C1, boolean isLocal)
```
Get the reference of this Name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the reference needs to be formatted as R1C1. |
| isLocal | boolean | Whether the reference needs to be formatted by locale. |
**Returns:**
java.lang.String
### getRefersTo(boolean isR1C1, boolean isLocal, int row, int column) {#getRefersTo-boolean-boolean-int-int-}
```
public String getRefersTo(boolean isR1C1, boolean isLocal, int row, int column)
```
Get the reference of this Name based on specified cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the reference needs to be formatted as R1C1. |
| isLocal | boolean | Whether the reference needs to be formatted by locale. |
| row | int | The row index of the cell. |
| column | int | The column index of the cell. |
**Returns:**
java.lang.String
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```
Indicates this name belongs to Workbook or Worksheet. 0 = Global name, otherwise index to sheet (one-based)
**Returns:**
int
### getText() {#getText--}
```
public String getText()
```
Gets the name text of the object.
**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isReferred() {#isReferred--}
```
public boolean isReferred()
```
Indicates whether this name is referred by other formulas.
**Returns:**
boolean
### isVisible() {#isVisible--}
```
public boolean isVisible()
```
Indicates whether the name is visible.
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
### setComment(String value) {#setComment-java.lang.String-}
```
public void setComment(String value)
```
Sets the comment of the name. Only applies for Excel 2007 or higher versions.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setR1C1RefersTo(String value) {#setR1C1RefersTo-java.lang.String-}
```
public void setR1C1RefersTo(String value)
```
Sets a R1C1 reference of the [Name](../../com.aspose.cells/name).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setRefersTo(String value) {#setRefersTo-java.lang.String-}
```
public void setRefersTo(String value)
```
Returns or sets the formula that the name is defined to refer to, beginning with an equal sign.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setRefersTo(String refersTo, boolean isR1C1, boolean isLocal) {#setRefersTo-java.lang.String-boolean-boolean-}
```
public void setRefersTo(String refersTo, boolean isR1C1, boolean isLocal)
```
Set the reference of this Name.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| refersTo | java.lang.String | The reference. |
| isR1C1 | boolean | Whether the reference is R1C1 format. |
| isLocal | boolean | Whether the reference is locale formatted. |
### setSheetIndex(int value) {#setSheetIndex-int-}
```
public void setSheetIndex(int value)
```
Indicates this name belongs to Workbook or Worksheet. 0 = Global name, otherwise index to sheet (one-based)
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```
Gets the name text of the object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```
Indicates whether the name is visible.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### toString() {#toString--}
```
public String toString()
```
Returns a string represents the current Range object.
**Returns:**
java.lang.String -
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
