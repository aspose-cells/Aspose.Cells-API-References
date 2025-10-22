##PivotFormatCondition
Represents a PivotTable Format Condition in PivotFormatCondition Collection.
## PivotFormatCondition class
Represents a PivotTable Format Condition in PivotFormatCondition Collection.
```javascript
class PivotFormatCondition;
```
### Remarks
NOTE: This class is now obsolete. Instead, please use [PivotConditionalFormat](../pivotconditionalformat/) class. This method will be removed 12 months later since December 2024. Aspose apologizes for any inconvenience you may have experienced.
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [scopeType](#scopeType--)| PivotConditionFormatScopeType | Get and set scope type for the pivot table conditional format . |
| [ruleType](#ruleType--)| PivotConditionFormatRuleType | Get and set rule type for the pivot table condition format . |
| [formatConditions](#formatConditions--)| FormatConditionCollection | Readonly. Get conditions for the pivot table conditional format . |
## Methods
| Method | Description |
| --- | --- |
| [getScopeType()](#getScopeType--)| <b>@deprecated.</b> Please use the 'scopeType' property instead. Get and set scope type for the pivot table conditional format . |
| [setScopeType(PivotConditionFormatScopeType)](#setScopeType-pivotconditionformatscopetype-)| <b>@deprecated.</b> Please use the 'scopeType' property instead. Get and set scope type for the pivot table conditional format . |
| [getRuleType()](#getRuleType--)| <b>@deprecated.</b> Please use the 'ruleType' property instead. Get and set rule type for the pivot table condition format . |
| [setRuleType(PivotConditionFormatRuleType)](#setRuleType-pivotconditionformatruletype-)| <b>@deprecated.</b> Please use the 'ruleType' property instead. Get and set rule type for the pivot table condition format . |
| [getFormatConditions()](#getFormatConditions--)| <b>@deprecated.</b> Please use the 'formatConditions' property instead. Get conditions for the pivot table conditional format . |
| [addDataAreaCondition(string)](#addDataAreaCondition-string-)| Adds PivotTable conditional format limit in the data fields. |
| [addDataAreaCondition(PivotField)](#addDataAreaCondition-pivotfield-)| Adds PivotTable conditional format limit in the data fields. |
| [addRowAreaCondition(string)](#addRowAreaCondition-string-)| Adds PivotTable conditional format limit in the row fields. |
| [addRowAreaCondition(PivotField)](#addRowAreaCondition-pivotfield-)| Adds PivotTable conditional format limit in the row fields. |
| [addColumnAreaCondition(string)](#addColumnAreaCondition-string-)| Adds PivotTable conditional format limit in the column fields. |
| [addColumnAreaCondition(PivotField)](#addColumnAreaCondition-pivotfield-)| Adds PivotTable conditional format limit in the column fields. |
| [setConditionalAreas()](#setConditionalAreas--)| Sets conditional areas of PivotFormatCondition object. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### formatConditions {#formatConditions--}
Readonly. Get conditions for the pivot table conditional format .
```javascript
formatConditions : FormatConditionCollection;
```
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
### getFormatConditions() {#getFormatConditions--}
```javascript
getFormatConditions() : FormatConditionCollection;
```
**Returns**
[FormatConditionCollection](../formatconditioncollection/)
### addDataAreaCondition(string) {#addDataAreaCondition-string-}
Adds PivotTable conditional format limit in the data fields.
```javascript
addDataAreaCondition(fieldName: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldName | string | The name of PivotField. |
### addDataAreaCondition(PivotField) {#addDataAreaCondition-pivotfield-}
Adds PivotTable conditional format limit in the data fields.
```javascript
addDataAreaCondition(dataField: PivotField) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| dataField | [PivotField](../pivotfield/) | The PivotField in the data fields. |
### addRowAreaCondition(string) {#addRowAreaCondition-string-}
Adds PivotTable conditional format limit in the row fields.
```javascript
addRowAreaCondition(fieldName: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldName | string | The name of PivotField. |
### addRowAreaCondition(PivotField) {#addRowAreaCondition-pivotfield-}
Adds PivotTable conditional format limit in the row fields.
```javascript
addRowAreaCondition(rowField: PivotField) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| rowField | [PivotField](../pivotfield/) | The PivotField in the row fields. |
### addColumnAreaCondition(string) {#addColumnAreaCondition-string-}
Adds PivotTable conditional format limit in the column fields.
```javascript
addColumnAreaCondition(fieldName: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fieldName | string | The name of PivotField. |
### addColumnAreaCondition(PivotField) {#addColumnAreaCondition-pivotfield-}
Adds PivotTable conditional format limit in the column fields.
```javascript
addColumnAreaCondition(columnField: PivotField) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| columnField | [PivotField](../pivotfield/) | The PivotField in the column fields. |
### setConditionalAreas() {#setConditionalAreas--}
Sets conditional areas of PivotFormatCondition object.
```javascript
setConditionalAreas() : void;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
