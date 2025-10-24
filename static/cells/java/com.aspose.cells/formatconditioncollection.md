##FormatConditionCollection
Represents conditional formatting.
**Inheritance:**
java.lang.Object
```
public class FormatConditionCollection
```
Represents conditional formatting. The FormatConditions can contain up to three conditional formats.
**Example**
```
//Create a new Workbook.
Workbook workbook = new Workbook();
//Get the first worksheet.
Worksheet sheet = workbook.getWorksheets().get(0);
//Adds an empty conditional formatting
int index = sheet.getConditionalFormattings().add();
FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
//Sets the conditional format range.
CellArea ca = new CellArea();
ca.StartRow = 0;
ca.EndRow = 0;
ca.StartColumn = 0;
ca.EndColumn = 0;
fcs.addArea(ca);
ca = new CellArea();
ca.StartRow = 1;
ca.EndRow = 1;
ca.StartColumn = 1;
ca.EndColumn = 1;
fcs.addArea(ca);
//Adds condition.
int conditionIndex = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100");
//Adds condition.
int conditionIndex2 = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100");
//Sets the background color.
FormatCondition fc = fcs.get(conditionIndex);
fc.getStyle().setBackgroundColor(Color.getRed());
//Saving the Excel file
workbook.save("output.xls");
```
## Methods
| Method | Description |
| --- | --- |
| [add(CellArea cellArea, int type, int operatorType, String formula1, String formula2)](#add-com.aspose.cells.CellArea-int-int-java.lang.String-java.lang.String-) | Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats. |
| [addArea(CellArea cellArea)](#addArea-com.aspose.cells.CellArea-) | Adds a conditional formatted cell range. |
| [addCondition(int type)](#addCondition-int-) | Add a format condition. |
| [addCondition(int type, int operatorType, String formula1, String formula2)](#addCondition-int-int-java.lang.String-java.lang.String-) | Adds a formatting condition. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the formatting condition by index. |
| [getCellArea(int index)](#getCellArea-int-) | Gets the conditional formatted cell range by index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the count of the conditions. |
| [getRangeCount()](#getRangeCount--) | Gets count of conditionally formatted ranges. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeArea(int index)](#removeArea-int-) | Removes conditional formatted cell range by index. |
| [removeArea(int startRow, int startColumn, int totalRows, int totalColumns)](#removeArea-int-int-int-int-) | Remove conditional formatting int the range. |
| [removeCondition(int index)](#removeCondition-int-) | Removes the formatting condition by index. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(CellArea cellArea, int type, int operatorType, String formula1, String formula2) {#add-com.aspose.cells.CellArea-int-int-java.lang.String-java.lang.String-}
```
public int[] add(CellArea cellArea, int type, int operatorType, String formula1, String formula2)
```
Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats. References to the other sheets are not allowed in the formulas of conditional formatting.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Conditional formatted cell range. |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Type of conditional formatting.It could be one of the members of FormatConditionType. |
| operatorType | int | [OperatorType](../../com.aspose.cells/operatortype). Comparison operator.It could be one of the members of OperatorType. |
| formula1 | java.lang.String | The value or expression associated with conditional formatting. |
| formula2 | java.lang.String | The value or expression associated with conditional formatting |
**Returns:**
int[] - [0]:Formatting condition object index;[1] Effected cell rang index.
### addArea(CellArea cellArea) {#addArea-com.aspose.cells.CellArea-}
```
public int addArea(CellArea cellArea)
```
Adds a conditional formatted cell range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Conditional formatted cell range. |
**Returns:**
int - Conditional formatted cell rang index.
### addCondition(int type) {#addCondition-int-}
```
public int addCondition(int type)
```
Add a format condition.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Format condition type. |
**Returns:**
int - Formatting condition object index;
### addCondition(int type, int operatorType, String formula1, String formula2) {#addCondition-int-int-java.lang.String-java.lang.String-}
```
public int addCondition(int type, int operatorType, String formula1, String formula2)
```
Adds a formatting condition.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). The type of format condition. |
| operatorType | int | [OperatorType](../../com.aspose.cells/operatortype). The operator type |
| formula1 | java.lang.String | The value or expression associated with conditional formatting. If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\\"=...\\"". |
| formula2 | java.lang.String | The value or expression associated with conditional formatting. The input format is same with formula1 |
**Returns:**
int - Formatting condition object index;
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
### get(int index) {#get-int-}
```
public FormatCondition get(int index)
```
Gets the formatting condition by index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | the index of the formatting condition to return. |
**Returns:**
[FormatCondition](../../com.aspose.cells/formatcondition) - the formatting condition
### getCellArea(int index) {#getCellArea-int-}
```
public CellArea getCellArea(int index)
```
Gets the conditional formatted cell range by index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | the index of the conditional formatted cell range. |
**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the conditional formatted cell range
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```
Gets the count of the conditions.
**Returns:**
int
### getRangeCount() {#getRangeCount--}
```
public int getRangeCount()
```
Gets count of conditionally formatted ranges.
**Returns:**
int
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
### removeArea(int index) {#removeArea-int-}
```
public void removeArea(int index)
```
Removes conditional formatted cell range by index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index of the conditional formatted cell range to be removed. |
### removeArea(int startRow, int startColumn, int totalRows, int totalColumns) {#removeArea-int-int-int-int-}
```
public boolean removeArea(int startRow, int startColumn, int totalRows, int totalColumns)
```
Remove conditional formatting int the range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | The startRow of the range. |
| startColumn | int | The startColumn of the range. |
| totalRows | int | The number of rows of the range. |
| totalColumns | int | The number of columns of the range. |
**Returns:**
boolean - Returns TRUE, this FormatCondtionCollection should be removed.
### removeCondition(int index) {#removeCondition-int-}
```
public void removeCondition(int index)
```
Removes the formatting condition by index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The index of the formatting condition to be removed. |
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
