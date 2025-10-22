##PivotArea
Presents the selected area of the PivotTable.
## PivotArea class
Presents the selected area of the PivotTable.
```javascript
class PivotArea;
```
## Constructors
| Constructor | Description |
| --- | --- |
| [constructor(PivotTable)](#constructor-pivottable-)| Presents the selected area of the PivotTable. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [filters](#filters--)| PivotAreaFilterCollection | Readonly. Gets all filters for this PivotArea. |
| [onlyData](#onlyData--)| boolean | Indicates whether only the data values (in the data area of the view) for an item selection are selected and does not include the item labels. |
| [onlyLabel](#onlyLabel--)| boolean | Indicates whether only the data labels for an item selection are selected. |
| [isRowGrandIncluded](#isRowGrandIncluded--)| boolean | Indicates whether the row grand total is included. |
| [isColumnGrandIncluded](#isColumnGrandIncluded--)| boolean | Indicates whether the column grand total is included. |
| [axisType](#axisType--)| PivotFieldType | Gets and sets the region of the PivotTable to which this rule applies. |
| [ruleType](#ruleType--)| PivotAreaType | Gets and sets the type of selection rule. |
| [isOutline](#isOutline--)| boolean | Indicates whether the rule refers to an area that is in outline mode. |
## Methods
| Method | Description |
| --- | --- |
| [getFilters()](#getFilters--)| <b>@deprecated.</b> Please use the 'filters' property instead. Gets all filters for this PivotArea. |
| [getOnlyData()](#getOnlyData--)| <b>@deprecated.</b> Please use the 'onlyData' property instead. Indicates whether only the data values (in the data area of the view) for an item selection are selected and does not include the item labels. |
| [setOnlyData(boolean)](#setOnlyData-boolean-)| <b>@deprecated.</b> Please use the 'onlyData' property instead. Indicates whether only the data values (in the data area of the view) for an item selection are selected and does not include the item labels. |
| [getOnlyLabel()](#getOnlyLabel--)| <b>@deprecated.</b> Please use the 'onlyLabel' property instead. Indicates whether only the data labels for an item selection are selected. |
| [setOnlyLabel(boolean)](#setOnlyLabel-boolean-)| <b>@deprecated.</b> Please use the 'onlyLabel' property instead. Indicates whether only the data labels for an item selection are selected. |
| [isRowGrandIncluded()](#isRowGrandIncluded--)| <b>@deprecated.</b> Please use the 'isRowGrandIncluded' property instead. Indicates whether the row grand total is included. |
| [setIsRowGrandIncluded(boolean)](#setIsRowGrandIncluded-boolean-)| <b>@deprecated.</b> Please use the 'isRowGrandIncluded' property instead. Indicates whether the row grand total is included. |
| [isColumnGrandIncluded()](#isColumnGrandIncluded--)| <b>@deprecated.</b> Please use the 'isColumnGrandIncluded' property instead. Indicates whether the column grand total is included. |
| [setIsColumnGrandIncluded(boolean)](#setIsColumnGrandIncluded-boolean-)| <b>@deprecated.</b> Please use the 'isColumnGrandIncluded' property instead. Indicates whether the column grand total is included. |
| [getAxisType()](#getAxisType--)| <b>@deprecated.</b> Please use the 'axisType' property instead. Gets and sets the region of the PivotTable to which this rule applies. |
| [setAxisType(PivotFieldType)](#setAxisType-pivotfieldtype-)| <b>@deprecated.</b> Please use the 'axisType' property instead. Gets and sets the region of the PivotTable to which this rule applies. |
| [getRuleType()](#getRuleType--)| <b>@deprecated.</b> Please use the 'ruleType' property instead. Gets and sets the type of selection rule. |
| [setRuleType(PivotAreaType)](#setRuleType-pivotareatype-)| <b>@deprecated.</b> Please use the 'ruleType' property instead. Gets and sets the type of selection rule. |
| [isOutline()](#isOutline--)| <b>@deprecated.</b> Please use the 'isOutline' property instead. Indicates whether the rule refers to an area that is in outline mode. |
| [setIsOutline(boolean)](#setIsOutline-boolean-)| <b>@deprecated.</b> Please use the 'isOutline' property instead. Indicates whether the rule refers to an area that is in outline mode. |
| [select(PivotFieldType, number, PivotTableSelectionType)](#select-pivotfieldtype-number-pivottableselectiontype-)| Select the area with filters. |
| [selectField(PivotFieldType, string)](#selectField-pivotfieldtype-string-)| Select a field in the region as an area. |
| [selectField(PivotFieldType, PivotField)](#selectField-pivotfieldtype-pivotfield-)| Select a field in the region as an area. |
| [getCellAreas()](#getCellAreas--)| Gets cell areas of this pivot area. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### constructor(PivotTable) {#constructor-pivottable-}
Presents the selected area of the PivotTable.
```javascript
constructor(table: PivotTable);
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| table | [PivotTable](../pivottable/) |  |
### filters {#filters--}
Readonly. Gets all filters for this PivotArea.
```javascript
filters : PivotAreaFilterCollection;
```
### onlyData {#onlyData--}
Indicates whether only the data values (in the data area of the view) for an item selection are selected and does not include the item labels.
```javascript
onlyData : boolean;
```
### onlyLabel {#onlyLabel--}
Indicates whether only the data labels for an item selection are selected.
```javascript
onlyLabel : boolean;
```
### isRowGrandIncluded {#isRowGrandIncluded--}
Indicates whether the row grand total is included.
```javascript
isRowGrandIncluded : boolean;
```
### isColumnGrandIncluded {#isColumnGrandIncluded--}
Indicates whether the column grand total is included.
```javascript
isColumnGrandIncluded : boolean;
```
### axisType {#axisType--}
Gets and sets the region of the PivotTable to which this rule applies.
```javascript
axisType : PivotFieldType;
```
### ruleType {#ruleType--}
Gets and sets the type of selection rule.
```javascript
ruleType : PivotAreaType;
```
### isOutline {#isOutline--}
Indicates whether the rule refers to an area that is in outline mode.
```javascript
isOutline : boolean;
```
### getFilters() {#getFilters--}
```javascript
getFilters() : PivotAreaFilterCollection;
```
**Returns**
[PivotAreaFilterCollection](../pivotareafiltercollection/)
### getOnlyData() {#getOnlyData--}
```javascript
getOnlyData() : boolean;
```
### setOnlyData(boolean) {#setOnlyData-boolean-}
```javascript
setOnlyData(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getOnlyLabel() {#getOnlyLabel--}
```javascript
getOnlyLabel() : boolean;
```
### setOnlyLabel(boolean) {#setOnlyLabel-boolean-}
```javascript
setOnlyLabel(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isRowGrandIncluded() {#isRowGrandIncluded--}
```javascript
isRowGrandIncluded() : boolean;
```
### setIsRowGrandIncluded(boolean) {#setIsRowGrandIncluded-boolean-}
```javascript
setIsRowGrandIncluded(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### isColumnGrandIncluded() {#isColumnGrandIncluded--}
```javascript
isColumnGrandIncluded() : boolean;
```
### setIsColumnGrandIncluded(boolean) {#setIsColumnGrandIncluded-boolean-}
```javascript
setIsColumnGrandIncluded(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAxisType() {#getAxisType--}
```javascript
getAxisType() : PivotFieldType;
```
**Returns**
[PivotFieldType](../pivotfieldtype/)
### setAxisType(PivotFieldType) {#setAxisType-pivotfieldtype-}
```javascript
setAxisType(value: PivotFieldType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotFieldType](../pivotfieldtype/) | The value to set. |
### getRuleType() {#getRuleType--}
```javascript
getRuleType() : PivotAreaType;
```
**Returns**
[PivotAreaType](../pivotareatype/)
### setRuleType(PivotAreaType) {#setRuleType-pivotareatype-}
```javascript
setRuleType(value: PivotAreaType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotAreaType](../pivotareatype/) | The value to set. |
### isOutline() {#isOutline--}
```javascript
isOutline() : boolean;
```
### setIsOutline(boolean) {#setIsOutline-boolean-}
```javascript
setIsOutline(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### select(PivotFieldType, number, PivotTableSelectionType) {#select-pivotfieldtype-number-pivottableselectiontype-}
Select the area with filters.
```javascript
select(axisType: PivotFieldType, fieldPosition: number, selectionType: PivotTableSelectionType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | [PivotFieldType](../pivotfieldtype/) | The region of the PivotTable to which this rule applies. |
| fieldPosition | number | Position of the field within the axis to which this rule applies. |
| selectionType | [PivotTableSelectionType](../pivottableselectiontype/) | Specifies what can be selected in a PivotTable during a structured selection. |
### selectField(PivotFieldType, string) {#selectField-pivotfieldtype-string-}
Select a field in the region as an area.
```javascript
selectField(axisType: PivotFieldType, fieldName: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | [PivotFieldType](../pivotfieldtype/) | The region type. |
| fieldName | string | The name of pivot field. |
### selectField(PivotFieldType, PivotField) {#selectField-pivotfieldtype-pivotfield-}
Select a field in the region as an area.
```javascript
selectField(axisType: PivotFieldType, field: PivotField) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | [PivotFieldType](../pivotfieldtype/) | The region type. |
| field | [PivotField](../pivotfield/) | The pivot field. |
### getCellAreas() {#getCellAreas--}
Gets cell areas of this pivot area.
```javascript
getCellAreas() : CellArea[];
```
**Returns**
[CellArea](../cellarea/)[]
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
