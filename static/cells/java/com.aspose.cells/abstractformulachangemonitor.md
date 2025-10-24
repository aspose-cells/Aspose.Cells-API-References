##AbstractFormulaChangeMonitor
Monitor for user to track the change of formulas during certain operations.
**Inheritance:**
java.lang.Object
```
public abstract class AbstractFormulaChangeMonitor
```
Monitor for user to track the change of formulas during certain operations.
**Remarks**
For example, while deleting/inserting range of cells, formulas of other cells may be changed because of the shift of references. Please note, methods in the monitor may be invoked multiple times for one object which contains the formula.
**Example**
```
class MyFormulaChangeMonitor extends AbstractFormulaChangeMonitor
{
private final WorksheetCollection mWorksheets;
public MyFormulaChangeMonitor(WorksheetCollection worksheets)
{
mWorksheets = worksheets;
}
public /*override*/ void onCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
{
System.out.println("Cell " + mWorksheets.get(sheetIndex).getName() + "!"
+ CellsHelper.cellIndexToName(rowIndex, columnIndex)
+ "'s formula was changed while inserting rows.");
}
}
Workbook wb = new Workbook("template.xlsx");
InsertOptions options = new InsertOptions();
options.setFormulaChangeMonitor(new MyFormulaChangeMonitor(wb.getWorksheets()));
wb.getWorksheets().get(0).getCells().insertRows(0, 2, options);
```
## Constructors
| Constructor | Description |
| --- | --- |
| [AbstractFormulaChangeMonitor()](#AbstractFormulaChangeMonitor--) |  |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [onCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)](#onCellFormulaChanged-int-int-int-) | The event that will be triggered when the formula in a cell is changed. |
| [onFormatConditionFormulaChanged(FormatCondition fc)](#onFormatConditionFormulaChanged-com.aspose.cells.FormatCondition-) | The event that will be triggered when the formula of FormatCondition is changed. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractFormulaChangeMonitor() {#AbstractFormulaChangeMonitor--}
```
public AbstractFormulaChangeMonitor()
```
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
### onCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex) {#onCellFormulaChanged-int-int-int-}
```
public void onCellFormulaChanged(int sheetIndex, int rowIndex, int columnIndex)
```
The event that will be triggered when the formula in a cell is changed.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | int | The sheet index of the changed cell |
| rowIndex | int | The row index of the changed cell |
| columnIndex | int | The column index of the changed cell |
### onFormatConditionFormulaChanged(FormatCondition fc) {#onFormatConditionFormulaChanged-com.aspose.cells.FormatCondition-}
```
public void onFormatConditionFormulaChanged(FormatCondition fc)
```
The event that will be triggered when the formula of FormatCondition is changed.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fc | [FormatCondition](../../com.aspose.cells/formatcondition) | The FormatCondition object whose formula is changed |
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
