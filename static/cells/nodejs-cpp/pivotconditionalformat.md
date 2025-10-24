##PivotConditionalFormat
Represents a PivotTable Format Condition in PivotFormatCondition Collection.
## PivotConditionalFormat class
Represents a PivotTable Format Condition in PivotFormatCondition Collection.
```javascript
class PivotConditionalFormat;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [pivotAreas](#pivotAreas--)| PivotAreaCollection | Readonly. Gets all pivot areas. |
| [formatConditions](#formatConditions--)| FormatConditionCollection | Readonly. Get conditions for the pivot table conditional format . |
| [scopeType](#scopeType--)| PivotConditionFormatScopeType | Get and set scope type for the pivot table conditional format . |
| [ruleType](#ruleType--)| PivotConditionFormatRuleType | Get and set rule type for the pivot table condition format . |
## Methods
| Method | Description |
| --- | --- |
| [getPivotAreas()](#getPivotAreas--)| <b>@deprecated.</b> Please use the 'pivotAreas' property instead. Gets all pivot areas. |
| [getFormatConditions()](#getFormatConditions--)| <b>@deprecated.</b> Please use the 'formatConditions' property instead. Get conditions for the pivot table conditional format . |
| [getScopeType()](#getScopeType--)| <b>@deprecated.</b> Please use the 'scopeType' property instead. Get and set scope type for the pivot table conditional format . |
| [setScopeType(PivotConditionFormatScopeType)](#setScopeType-pivotconditionformatscopetype-)| <b>@deprecated.</b> Please use the 'scopeType' property instead. Get and set scope type for the pivot table conditional format . |
| [getRuleType()](#getRuleType--)| <b>@deprecated.</b> Please use the 'ruleType' property instead. Get and set rule type for the pivot table condition format . |
| [setRuleType(PivotConditionFormatRuleType)](#setRuleType-pivotconditionformatruletype-)| <b>@deprecated.</b> Please use the 'ruleType' property instead. Get and set rule type for the pivot table condition format . |
| [getCellAreas()](#getCellAreas--)| Gets all cell areas where this conditional format applies to. |
| [addCellArea(CellArea)](#addCellArea-cellarea-)| Adds an area based on pivot table view. |
| [applyTo(number, number, PivotConditionFormatScopeType)](#applyTo-number-number-pivotconditionformatscopetype-)| Applies the conditional format to range. Only for the data region. |
| [addFieldArea(PivotFieldType, string)](#addFieldArea-pivotfieldtype-string-)| Adds an area of pivot field. |
| [addFieldArea(PivotFieldType, PivotField)](#addFieldArea-pivotfieldtype-pivotfield-)| Adds an area of pivot field. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### pivotAreas {#pivotAreas--}
Readonly. Gets all pivot areas.
```javascript
pivotAreas : PivotAreaCollection;
```
### formatConditions {#formatConditions--}
Readonly. Get conditions for the pivot table conditional format .
```javascript
formatConditions : FormatConditionCollection;
```
### scopeType {#scopeType--}
Get and set scope type for the pivot table conditional format .
```javascript
scopeType : PivotConditionFormatScopeType;
```
### ruleType {#ruleType--}
Get and set rule type for the pivot table condition format .
```javascript
ruleType : PivotConditionFormatRuleType;
```
### getPivotAreas() {#getPivotAreas--}
```javascript
getPivotAreas() : PivotAreaCollection;
```
**Returns**
[PivotAreaCollection](../pivotareacollection/)
### getFormatConditions() {#getFormatConditions--}
```javascript
getFormatConditions() : FormatConditionCollection;
```
**Returns**
[FormatConditionCollection](../formatconditioncollection/)
### getScopeType() {#getScopeType--}
```javascript
getScopeType() : PivotConditionFormatScopeType;
```
**Returns**
[PivotConditionFormatScopeType](../pivotconditionformatscopetype/)
### setScopeType(PivotConditionFormatScopeType) {#setScopeType-pivotconditionformatscopetype-}
```javascript
setScopeType(value: PivotConditionFormatScopeType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotConditionFormatScopeType](../pivotconditionformatscopetype/) | The value to set. |
### getRuleType() {#getRuleType--}
```javascript
getRuleType() : PivotConditionFormatRuleType;
```
**Returns**
[PivotConditionFormatRuleType](../pivotconditionformatruletype/)
### setRuleType(PivotConditionFormatRuleType) {#setRuleType-pivotconditionformatruletype-}
```javascript
setRuleType(value: PivotConditionFormatRuleType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [PivotConditionFormatRuleType](../pivotconditionformatruletype/) | The value to set. |
### getCellAreas() {#getCellAreas--}
Gets all cell areas where this conditional format applies to.
```javascript
getCellAreas() : CellArea[];
```
**Returns**
[CellArea](../cellarea/)[]
### addCellArea(CellArea) {#addCellArea-cellarea-}
Adds an area based on pivot table view.
```javascript
addCellArea(ca: CellArea) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../cellarea/) | The cell area. |
### applyTo(number, number, PivotConditionFormatScopeType) {#applyTo-number-number-pivotconditionformatscopetype-}
Applies the conditional format to range. Only for the data region.
```javascript
applyTo(row: number, column: number, scope: PivotConditionFormatScopeType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The selected row. |
| column | number | The selected column. |
| scope | [PivotConditionFormatScopeType](../pivotconditionformatscopetype/) | The scope |
### addFieldArea(PivotFieldType, string) {#addFieldArea-pivotfieldtype-string-}
Adds an area of pivot field.
```javascript
addFieldArea(axisType: PivotFieldType, fieldName: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | [PivotFieldType](../pivotfieldtype/) | The region type. |
| fieldName | string | The name of pivot field. |
### addFieldArea(PivotFieldType, PivotField) {#addFieldArea-pivotfieldtype-pivotfield-}
Adds an area of pivot field.
```javascript
addFieldArea(axisType: PivotFieldType, field: PivotField) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | [PivotFieldType](../pivotfieldtype/) | The region type. |
| field | [PivotField](../pivotfield/) | The pivot field. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
