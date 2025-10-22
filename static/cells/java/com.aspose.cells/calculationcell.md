##CalculationCell
Represents the calculation relevant data about one cell which is being calculated.
**Inheritance:**
java.lang.Object
```
public class CalculationCell
```
Represents the calculation relevant data about one cell which is being calculated.
**Remarks**
All objects provided by this class are for "read" purpose only. User should not change any data in the Workbook during the formula calculation process, Otherwise unexpected result or Exception may be caused.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCell()](#getCell--) | Gets the Cell object which is being calculated. |
| [getCellColumn()](#getCellColumn--) | Gets the column index of the cell. |
| [getCellRow()](#getCellRow--) | Gets the row index of the cell. |
| [getClass()](#getClass--) |  |
| [getWorkbook()](#getWorkbook--) | Gets the Workbook object. |
| [getWorksheet()](#getWorksheet--) | Gets the Worksheet object where the cell is in. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object v)](#setCalculatedValue-java.lang.Object-) | Sets the calculated value for the cell. |
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
### getCell() {#getCell--}
```
public Cell getCell()
```
Gets the Cell object which is being calculated.
**Returns:**
[Cell](../../com.aspose.cells/cell)
### getCellColumn() {#getCellColumn--}
```
public int getCellColumn()
```
Gets the column index of the cell.
**Returns:**
int
### getCellRow() {#getCellRow--}
```
public int getCellRow()
```
Gets the row index of the cell.
**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```
Gets the Workbook object.
**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```
Gets the Worksheet object where the cell is in.
**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
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
### setCalculatedValue(Object v) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object v)
```
Sets the calculated value for the cell.
**Remarks**
User can set the calculated result by this method to ignore the automatic calculation for the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| v | java.lang.Object |  |
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
