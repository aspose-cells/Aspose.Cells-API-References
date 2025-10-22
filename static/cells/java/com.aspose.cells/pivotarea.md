##PivotArea
Presents the selected area of the PivotTable.
**Inheritance:**
java.lang.Object
```
public class PivotArea
```
Presents the selected area of the PivotTable.
## Constructors
| Constructor | Description |
| --- | --- |
| [PivotArea(PivotTable table)](#PivotArea-com.aspose.cells.PivotTable-) | Presents the selected area of the PivotTable. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAxisType()](#getAxisType--) | Gets the region of the PivotTable to which this rule applies. |
| [getCellAreas()](#getCellAreas--) | Gets cell areas of this pivot area. |
| [getClass()](#getClass--) |  |
| [getFilters()](#getFilters--) | Gets all filters for this PivotArea. |
| [getOnlyData()](#getOnlyData--) | Indicates whether only the data values (in the data area of the view) for an item selection are selected and does not include the item labels. |
| [getOnlyLabel()](#getOnlyLabel--) | Indicates whether only the data labels for an item selection are selected. |
| [getRuleType()](#getRuleType--) | Gets the type of selection rule. |
| [hashCode()](#hashCode--) |  |
| [isColumnGrandIncluded()](#isColumnGrandIncluded--) | Indicates whether the column grand total is included. |
| [isOutline()](#isOutline--) | Indicates whether the rule refers to an area that is in outline mode. |
| [isRowGrandIncluded()](#isRowGrandIncluded--) | Indicates whether the row grand total is included. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [select(int axisType, int fieldPosition, int selectionType)](#select-int-int-int-) | Select the area with filters. |
| [selectField(int axisType, PivotField field)](#selectField-int-com.aspose.cells.PivotField-) | Select a field in the region as an area. |
| [selectField(int axisType, String fieldName)](#selectField-int-java.lang.String-) | Select a field in the region as an area. |
| [setAxisType(int value)](#setAxisType-int-) | Sets the region of the PivotTable to which this rule applies. |
| [setColumnGrandIncluded(boolean value)](#setColumnGrandIncluded-boolean-) | Indicates whether the column grand total is included. |
| [setOnlyData(boolean value)](#setOnlyData-boolean-) | Indicates whether only the data values (in the data area of the view) for an item selection are selected and does not include the item labels. |
| [setOnlyLabel(boolean value)](#setOnlyLabel-boolean-) | Indicates whether only the data labels for an item selection are selected. |
| [setOutline(boolean value)](#setOutline-boolean-) | Indicates whether the rule refers to an area that is in outline mode. |
| [setRowGrandIncluded(boolean value)](#setRowGrandIncluded-boolean-) | Indicates whether the row grand total is included. |
| [setRuleType(int value)](#setRuleType-int-) | Sets the type of selection rule. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotArea(PivotTable table) {#PivotArea-com.aspose.cells.PivotTable-}
```
public PivotArea(PivotTable table)
```
Presents the selected area of the PivotTable.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| table | [PivotTable](../../com.aspose.cells/pivottable) |  |
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
### getAxisType() {#getAxisType--}
```
public int getAxisType()
```
Gets the region of the PivotTable to which this rule applies.
See [PivotFieldType](../../com.aspose.cells/pivotfieldtype).
**Returns:**
int
### getCellAreas() {#getCellAreas--}
```
public CellArea[] getCellAreas()
```
Gets cell areas of this pivot area.
**Returns:**
com.aspose.cells.CellArea[] -
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getFilters() {#getFilters--}
```
public PivotAreaFilterCollection getFilters()
```
Gets all filters for this PivotArea.
**Returns:**
[PivotAreaFilterCollection](../../com.aspose.cells/pivotareafiltercollection)
### getOnlyData() {#getOnlyData--}
```
public boolean getOnlyData()
```
Indicates whether only the data values (in the data area of the view) for an item selection are selected and does not include the item labels.
**Returns:**
boolean
### getOnlyLabel() {#getOnlyLabel--}
```
public boolean getOnlyLabel()
```
Indicates whether only the data labels for an item selection are selected.
**Returns:**
boolean
### getRuleType() {#getRuleType--}
```
public int getRuleType()
```
Gets the type of selection rule.
See [PivotAreaType](../../com.aspose.cells/pivotareatype).
**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isColumnGrandIncluded() {#isColumnGrandIncluded--}
```
public boolean isColumnGrandIncluded()
```
Indicates whether the column grand total is included.
**Returns:**
boolean
### isOutline() {#isOutline--}
```
public boolean isOutline()
```
Indicates whether the rule refers to an area that is in outline mode.
**Returns:**
boolean
### isRowGrandIncluded() {#isRowGrandIncluded--}
```
public boolean isRowGrandIncluded()
```
Indicates whether the row grand total is included.
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
### select(int axisType, int fieldPosition, int selectionType) {#select-int-int-int-}
```
public void select(int axisType, int fieldPosition, int selectionType)
```
Select the area with filters.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). The region of the PivotTable to which this rule applies. |
| fieldPosition | int | Position of the field within the axis to which this rule applies. |
| selectionType | int | [PivotTableSelectionType](../../com.aspose.cells/pivottableselectiontype). Specifies what can be selected in a PivotTable during a structured selection. |
### selectField(int axisType, PivotField field) {#selectField-int-com.aspose.cells.PivotField-}
```
public void selectField(int axisType, PivotField field)
```
Select a field in the region as an area.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). The region type. |
| field | [PivotField](../../com.aspose.cells/pivotfield) | The pivot field. |
### selectField(int axisType, String fieldName) {#selectField-int-java.lang.String-}
```
public void selectField(int axisType, String fieldName)
```
Select a field in the region as an area.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | int | [PivotFieldType](../../com.aspose.cells/pivotfieldtype). The region type. |
| fieldName | java.lang.String | The name of pivot field. |
### setAxisType(int value) {#setAxisType-int-}
```
public void setAxisType(int value)
```
Sets the region of the PivotTable to which this rule applies.
See [PivotFieldType](../../com.aspose.cells/pivotfieldtype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setColumnGrandIncluded(boolean value) {#setColumnGrandIncluded-boolean-}
```
public void setColumnGrandIncluded(boolean value)
```
Indicates whether the column grand total is included.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setOnlyData(boolean value) {#setOnlyData-boolean-}
```
public void setOnlyData(boolean value)
```
Indicates whether only the data values (in the data area of the view) for an item selection are selected and does not include the item labels.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setOnlyLabel(boolean value) {#setOnlyLabel-boolean-}
```
public void setOnlyLabel(boolean value)
```
Indicates whether only the data labels for an item selection are selected.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setOutline(boolean value) {#setOutline-boolean-}
```
public void setOutline(boolean value)
```
Indicates whether the rule refers to an area that is in outline mode.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setRowGrandIncluded(boolean value) {#setRowGrandIncluded-boolean-}
```
public void setRowGrandIncluded(boolean value)
```
Indicates whether the row grand total is included.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setRuleType(int value) {#setRuleType-int-}
```
public void setRuleType(int value)
```
Sets the type of selection rule.
See [PivotAreaType](../../com.aspose.cells/pivotareatype).
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
