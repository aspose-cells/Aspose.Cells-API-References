##PivotConditionalFormat
Represents a PivotTable Format Condition in PivotFormatCondition Collection.
**Inheritance:**
java.lang.Object
```
public class PivotConditionalFormat
```
Represents a PivotTable Format Condition in PivotFormatCondition Collection.
**Example**
```
Workbook book = new Workbook();
Worksheet sheet = book.getWorksheets().get(0);
Cells cells = sheet.getCells();
cells.get(0, 0).setValue("fruit");
cells.get(1, 0).setValue("grape");
cells.get(2, 0).setValue("blueberry");
cells.get(3, 0).setValue("kiwi");
cells.get(4, 0).setValue("cherry");
cells.get(5, 0).setValue("grape");
cells.get(6, 0).setValue("blueberry");
cells.get(7, 0).setValue("kiwi");
cells.get(8, 0).setValue("cherry");
cells.get(0, 1).setValue("year");
cells.get(1, 1).setValue(2020);
cells.get(2, 1).setValue(2020);
cells.get(3, 1).setValue(2020);
cells.get(4, 1).setValue(2020);
cells.get(5, 1).setValue(2021);
cells.get(6, 1).setValue(2021);
cells.get(7, 1).setValue(2021);
cells.get(8, 1).setValue(2021);
cells.get(0, 2).setValue("amount");
cells.get(1, 2).setValue(50);
cells.get(2, 2).setValue(60);
cells.get(3, 2).setValue(70);
cells.get(4, 2).setValue(80);
cells.get(5, 2).setValue(90);
cells.get(6, 2).setValue(100);
cells.get(7, 2).setValue(110);
cells.get(8, 2).setValue(120);
PivotTableCollection pivots = sheet.getPivotTables();
int pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable");
PivotTable pivot = pivots.get(pivotIndex);
pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
pivot.addFieldToArea(PivotFieldType.DATA, "amount");
pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
//Add PivotFormatCondition
int formatIndex = pivot.getConditionalFormats().add();
PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
pfc.addFieldArea(PivotFieldType.DATA, pivot.getDataFields().get(0));
int idx = pfc.getFormatConditions().addCondition(FormatConditionType.CELL_VALUE);
FormatCondition fc = pfc.getFormatConditions().get(idx);
fc.setFormula1("100");
fc.setOperator(OperatorType.GREATER_OR_EQUAL);
fc.getStyle().setBackgroundColor(Color.getRed());
pivot.refreshData();
pivot.calculateData();
//do your business
book.save("out.xlsx");
```
## Methods
| Method | Description |
| --- | --- |
| [addCellArea(CellArea ca)](#addCellArea-com.aspose.cells.CellArea-) | Adds an area based on pivot table view. |
| [addFieldArea(int axisType, PivotField field)](#addFieldArea-int-com.aspose.cells.PivotField-) | Adds an area of pivot field. |
| [addFieldArea(int axisType, String fieldName)](#addFieldArea-int-java.lang.String-) | Adds an area of pivot field. |
| [applyTo(int row, int column, int scope)](#applyTo-int-int-int-) | Applies the conditional format to range. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCellAreas()](#getCellAreas--) | Gets all cell areas where this conditional format applies to. |
| [getClass()](#getClass--) |  |
| [getFormatConditions()](#getFormatConditions--) | Get conditions for the pivot table conditional format . |
| [getPivotAreas()](#getPivotAreas--) | Gets all pivot areas. |
| [getRuleType()](#getRuleType--) | Gets rule type for the pivot table condition format . |
| [getScopeType()](#getScopeType--) | Gets scope type for the pivot table conditional format . |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setRuleType(int value)](#setRuleType-int-) | Sets rule type for the pivot table condition format . |
| [setScopeType(int value)](#setScopeType-int-) | Sets scope type for the pivot table conditional format . |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addCellArea(CellArea ca) {#addCellArea-com.aspose.cells.CellArea-}
```
public void addCellArea(CellArea ca)
```
Adds an area based on pivot table view.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | The cell area. |
### addFieldArea(int axisType, PivotField field) {#addFieldArea-int-com.aspose.cells.PivotField-}
```
public void addFieldArea(int axisType, PivotField field)
```
Adds an area of pivot field.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). The region type. |
| field | [PivotField](../../com.aspose.cells/pivotfield) | The pivot field. |
### addFieldArea(int axisType, String fieldName) {#addFieldArea-int-java.lang.String-}
```
public void addFieldArea(int axisType, String fieldName)
```
Adds an area of pivot field.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). The region type. |
| fieldName | java.lang.String | The name of pivot field. |
### applyTo(int row, int column, int scope) {#applyTo-int-int-int-}
```
public void applyTo(int row, int column, int scope)
```
Applies the conditional format to range. Only for the data region.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The selected row. |
| column | int | The selected column. |
| scope | int | [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype). The scope |
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
### getCellAreas() {#getCellAreas--}
```
public CellArea[] getCellAreas()
```
Gets all cell areas where this conditional format applies to.
**Returns:**
com.aspose.cells.CellArea[] -
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getFormatConditions() {#getFormatConditions--}
```
public FormatConditionCollection getFormatConditions()
```
Get conditions for the pivot table conditional format .
**Returns:**
[FormatConditionCollection](../../com.aspose.cells/formatconditioncollection)
### getPivotAreas() {#getPivotAreas--}
```
public PivotAreaCollection getPivotAreas()
```
Gets all pivot areas.
**Returns:**
[PivotAreaCollection](../../com.aspose.cells/pivotareacollection)
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```
Gets rule type for the pivot table condition format .
See [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).
**Returns:**
int
### getScopeType() {#getScopeType--}
```
public int getScopeType()
```
Gets scope type for the pivot table conditional format .
See [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).
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
### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```
Sets rule type for the pivot table condition format .
See [PivotConditionFormatRuleType](../../com.aspose.cells/pivotconditionformatruletype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setScopeType(int value) {#setScopeType-int-}
```
public void setScopeType(int value)
```
Sets scope type for the pivot table conditional format .
See [PivotConditionFormatScopeType](../../com.aspose.cells/pivotconditionformatscopetype).
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
