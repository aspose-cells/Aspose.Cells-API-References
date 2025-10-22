##PivotAreaFilter
Represents the filter of PivotArea..pivotarea for PivotTable..pivottable.
## PivotAreaFilter class
Represents the filter of [PivotArea](../pivotarea/) for [PivotTable](../pivottable/).
```javascript
class PivotAreaFilter;
```
## Constructors
| Name | Description |
| --- | --- |
| [constructor()](#constructor--)| Default Constructor. |
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [selected](#selected--)| boolean | Indicates whether this field has selection. Only works when the PivotTable is in Outline view. |
## Methods
| Method | Description |
| --- | --- |
| [isSubtotalSet(PivotFieldSubtotalType)](#isSubtotalSet-pivotfieldsubtotaltype-)| Gets which subtotal is set for this filter. |
| [setSubtotals(PivotFieldSubtotalType, boolean)](#setSubtotals-pivotfieldsubtotaltype-boolean-)| Subtotal for the filter. |
### constructor() {#constructor--}
Default Constructor.
```javascript
constructor();
```
### selected {#selected--}
Indicates whether this field has selection. Only works when the PivotTable is in Outline view.
```javascript
selected : boolean;
```
### isSubtotalSet(PivotFieldSubtotalType) {#isSubtotalSet-pivotfieldsubtotaltype-}
Gets which subtotal is set for this filter.
```javascript
isSubtotalSet(subtotalType: PivotFieldSubtotalType) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | [PivotFieldSubtotalType](../pivotfieldsubtotaltype/) | The subtotal function type. |
### setSubtotals(PivotFieldSubtotalType, boolean) {#setSubtotals-pivotfieldsubtotaltype-boolean-}
Subtotal for the filter.
```javascript
setSubtotals(subtotalType: PivotFieldSubtotalType, shown: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| subtotalType | [PivotFieldSubtotalType](../pivotfieldsubtotaltype/) | The subtotal function. |
| shown | boolean | Indicates if showing this subtotal data. |
