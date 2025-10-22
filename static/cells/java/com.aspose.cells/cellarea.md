##CellArea
Represent an area of cells.
**Inheritance:**
java.lang.Object
**All Implemented Interfaces:**
java.lang.Comparable
```
public final class CellArea implements Comparable
```
Represent an area of cells.
**Example**
```
//Create Cell Area
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 0;
ca.StartColumn = 0;
ca.EndColumn = 0;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [CellArea()](#CellArea--) |  |
## Fields
| Field | Description |
| --- | --- |
| [EndColumn](#EndColumn) | Gets or set the end column of this area. |
| [EndRow](#EndRow) | Gets or set the end row of this area. |
| [StartColumn](#StartColumn) | Gets or set the start column of this area. |
| [StartRow](#StartRow) | Gets or set the start row of this area. |
## Methods
| Method | Description |
| --- | --- |
| [compareTo(Object obj)](#compareTo-java.lang.Object-) | Compare two CellArea objects according to their top-left corner. |
| [createCellArea(int startRow, int startColumn, int endRow, int endColumn)](#createCellArea-int-int-int-int-) | Creates a cell area. |
| [createCellArea(String startCellName, String endCellName)](#createCellArea-java.lang.String-java.lang.String-) | Creates a cell area. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | Returns a string represents the current cell area object. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CellArea() {#CellArea--}
```
public CellArea()
```
### EndColumn {#EndColumn}
```
public int EndColumn
```
Gets or set the end column of this area.
### EndRow {#EndRow}
```
public int EndRow
```
Gets or set the end row of this area.
### StartColumn {#StartColumn}
```
public int StartColumn
```
Gets or set the start column of this area.
### StartRow {#StartRow}
```
public int StartRow
```
Gets or set the start row of this area.
### compareTo(Object obj) {#compareTo-java.lang.Object-}
```
public int compareTo(Object obj)
```
Compare two CellArea objects according to their top-left corner.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object |  |
**Returns:**
int - If two corners are in different rows, then compare their row index. Otherwise compare their column index. If two corners are same, then 0 will be returned.
### createCellArea(int startRow, int startColumn, int endRow, int endColumn) {#createCellArea-int-int-int-int-}
```
public static CellArea createCellArea(int startRow, int startColumn, int endRow, int endColumn)
```
Creates a cell area.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | The start row. |
| startColumn | int | The start column. |
| endRow | int | The end row. |
| endColumn | int | The end column. |
**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Return a [CellArea](../../com.aspose.cells/cellarea).
### createCellArea(String startCellName, String endCellName) {#createCellArea-java.lang.String-java.lang.String-}
```
public static CellArea createCellArea(String startCellName, String endCellName)
```
Creates a cell area.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startCellName | java.lang.String | The top-left cell of the range. |
| endCellName | java.lang.String | The bottom-right cell of the range. |
**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Return a [CellArea](../../com.aspose.cells/cellarea).
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
### toString() {#toString--}
```
public String toString()
```
Returns a string represents the current cell area object.
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
