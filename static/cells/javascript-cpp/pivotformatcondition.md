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
| [addDataAreaCondition(string)](#addDataAreaCondition-string-)| Adds PivotTable conditional format limit in the data fields. |
| [addDataAreaCondition(PivotField)](#addDataAreaCondition-pivotfield-)| Adds PivotTable conditional format limit in the data fields. |
| [addRowAreaCondition(string)](#addRowAreaCondition-string-)| Adds PivotTable conditional format limit in the row fields. |
| [addRowAreaCondition(PivotField)](#addRowAreaCondition-pivotfield-)| Adds PivotTable conditional format limit in the row fields. |
| [addColumnAreaCondition(string)](#addColumnAreaCondition-string-)| Adds PivotTable conditional format limit in the column fields. |
| [addColumnAreaCondition(PivotField)](#addColumnAreaCondition-pivotfield-)| Adds PivotTable conditional format limit in the column fields. |
| [setConditionalAreas()](#setConditionalAreas--)| Sets conditional areas of PivotFormatCondition object. |
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
