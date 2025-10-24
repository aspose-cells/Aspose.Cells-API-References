##ListColumn
Represents a column in a Table.
**Inheritance:**
java.lang.Object
```
public class ListColumn
```
Represents a column in a Table.
**Example**
```
Workbook workbook = new Workbook();
Cells cells = workbook.getWorksheets().get(0).getCells();
for (int i = 0; i  ? i++)
{
cells.get(0,i).putValue(CellsHelper.columnIndexToName(i));
}
for (int row = 1; row  ? row++)
{
for (int column = 0; column  ? column++)
{
cells.get(row, column).putValue(row * column);
}
}
ListObjectCollection tables = workbook.getWorksheets().get(0).getListObjects();
int index = tables.add(0, 0, 9, 4, true);
ListObject table = tables.get(0);
table.setShowTotals(true);
ListColumn listColumn = table.getListColumns().get(4);
listColumn.setTotalsCalculation(com.aspose.cells.TotalsCalculation.SUM);
listColumn.setFormula("=[A]");
workbook.save("Book1.xlsx");
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCustomCalculatedFormula(boolean isR1C1, boolean isLocal)](#getCustomCalculatedFormula-boolean-boolean-) | Gets the formula of this list column. |
| [getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal)](#getCustomTotalsRowFormula-boolean-boolean-) | Gets the formula of totals row of this list column. |
| [getDataStyle()](#getDataStyle--) | Gets the style of the data in this column of the table. |
| [getFormula()](#getFormula--) | Gets the formula of the list column. |
| [getName()](#getName--) | Gets the name of the column. |
| [getRange()](#getRange--) | Gets the range of this list column. |
| [getTotalsCalculation()](#getTotalsCalculation--) | Gets the type of calculation in the Totals row of the list column. |
| [getTotalsRowLabel()](#getTotalsRowLabel--) | Gets the display labels of total row. |
| [hashCode()](#hashCode--) |  |
| [isArrayFormula()](#isArrayFormula--) | Indicates whether the fomula is array formula. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal)](#setCustomCalculatedFormula-java.lang.String-boolean-boolean-) | Sets the formula for this list column. |
| [setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal)](#setCustomTotalsRowFormula-java.lang.String-boolean-boolean-) | Gets the formula of totals row of this list column. |
| [setDataStyle(Style style)](#setDataStyle-com.aspose.cells.Style-) | Sets the style of the data in this column of the table. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Sets the formula of the list column. |
| [setName(String value)](#setName-java.lang.String-) | Sets the name of the column. |
| [setTotalsCalculation(int value)](#setTotalsCalculation-int-) | Sets the type of calculation in the Totals row of the list column. |
| [setTotalsRowLabel(String value)](#setTotalsRowLabel-java.lang.String-) | Sets the display labels of total row. |
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getCustomCalculatedFormula(boolean isR1C1, boolean isLocal) {#getCustomCalculatedFormula-boolean-boolean-}
```
public String getCustomCalculatedFormula(boolean isR1C1, boolean isLocal)
```
Gets the formula of this list column.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
**Returns:**
java.lang.String - The formula of this list column.
### getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal) {#getCustomTotalsRowFormula-boolean-boolean-}
```
public String getCustomTotalsRowFormula(boolean isR1C1, boolean isLocal)
```
Gets the formula of totals row of this list column.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
**Returns:**
java.lang.String - The formula of this list column.
### getDataStyle() {#getDataStyle--}
```
public Style getDataStyle()
```
Gets the style of the data in this column of the table.
**Returns:**
[Style](../../com.aspose.cells/style)
### getFormula() {#getFormula--}
```
public String getFormula()
```
Gets the formula of the list column.
**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```
Gets the name of the column.
**Remarks**
If sets the name of the column, the according cell' value will be changed too.
**Returns:**
java.lang.String
### getRange() {#getRange--}
```
public Range getRange()
```
Gets the range of this list column.
**Returns:**
[Range](../../com.aspose.cells/range)
### getTotalsCalculation() {#getTotalsCalculation--}
```
public int getTotalsCalculation()
```
Gets the type of calculation in the Totals row of the list column.
See [TotalsCalculation](../../com.aspose.cells/totalscalculation).
**Returns:**
int
### getTotalsRowLabel() {#getTotalsRowLabel--}
```
public String getTotalsRowLabel()
```
Gets the display labels of total row.
**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isArrayFormula() {#isArrayFormula--}
```
public boolean isArrayFormula()
```
Indicates whether the fomula is array formula.
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
### setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal) {#setCustomCalculatedFormula-java.lang.String-boolean-boolean-}
```
public void setCustomCalculatedFormula(String formula, boolean isR1C1, boolean isLocal)
```
Sets the formula for this list column.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | the formula for this list column. |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
### setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal) {#setCustomTotalsRowFormula-java.lang.String-boolean-boolean-}
```
public void setCustomTotalsRowFormula(String formula, boolean isR1C1, boolean isLocal)
```
Gets the formula of totals row of this list column.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | the formula for this list column. |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
### setDataStyle(Style style) {#setDataStyle-com.aspose.cells.Style-}
```
public void setDataStyle(Style style)
```
Sets the style of the data in this column of the table.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../../com.aspose.cells/style) |  |
### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```
Sets the formula of the list column.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```
Sets the name of the column.
**Remarks**
If sets the name of the column, the according cell' value will be changed too.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setTotalsCalculation(int value) {#setTotalsCalculation-int-}
```
public void setTotalsCalculation(int value)
```
Sets the type of calculation in the Totals row of the list column.
See [TotalsCalculation](../../com.aspose.cells/totalscalculation).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setTotalsRowLabel(String value) {#setTotalsRowLabel-java.lang.String-}
```
public void setTotalsRowLabel(String value)
```
Sets the display labels of total row.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
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
