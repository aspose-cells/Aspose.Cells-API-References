##PivotTableFormatCollection
Represents the collection of formats applied to PivotTable.
## PivotTableFormatCollection class
Represents the collection of formats applied to PivotTable.
```javascript
class PivotTableFormatCollection;
```
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the format by the index. |
| [add()](#add--)| Add a [PivotTableFormat](../pivottableformat/). |
| [formatArea(PivotFieldType, number, PivotFieldSubtotalType, PivotTableSelectionType, boolean, boolean, Style)](#formatArea-pivotfieldtype-number-pivotfieldsubtotaltype-pivottableselectiontype-boolean-boolean-style-)| Formats selected area. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the number of elements contained in. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### get(number) {#get-number-}
Gets the format by the index.
```javascript
get(index: number) : PivotTableFormat;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index. |
**Returns**
[PivotTableFormat](../pivottableformat/)
### add() {#add--}
Add a [PivotTableFormat](../pivottableformat/).
```javascript
add() : number;
```
**Returns**
The index of new format.
### formatArea(PivotFieldType, number, PivotFieldSubtotalType, PivotTableSelectionType, boolean, boolean, Style) {#formatArea-pivotfieldtype-number-pivotfieldsubtotaltype-pivottableselectiontype-boolean-boolean-style-}
Formats selected area.
```javascript
formatArea(axisType: PivotFieldType, fieldPosition: number, subtotalType: PivotFieldSubtotalType, selectionType: PivotTableSelectionType, isGrandRow: boolean, isGrandColumn: boolean, style: Style) : PivotTableFormat;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | [PivotFieldType](../pivotfieldtype/) | The region of the PivotTable to which this rule applies. |
| fieldPosition | number | Position of the field within the axis to which this rule applies. |
| subtotalType | [PivotFieldSubtotalType](../pivotfieldsubtotaltype/) | The subtotal filter type of the pivot field |
| selectionType | [PivotTableSelectionType](../pivottableselectiontype/) | Indicates how to select data. |
| isGrandRow | boolean | Indicates whether selecting grand total rows. |
| isGrandColumn | boolean | Indicates whether selecting grand total columns. |
| style | [Style](../style/) | The style which appies to the area of the pivot table. |
**Returns**
[PivotTableFormat](../pivottableformat/)
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
