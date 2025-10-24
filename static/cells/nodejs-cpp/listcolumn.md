##ListColumn
Represents a column in a Table.
## ListColumn class
Represents a column in a Table.
```javascript
class ListColumn;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [name](#name--)| string | Gets and sets the name of the column. |
| [totalsCalculation](#totalsCalculation--)| TotalsCalculation | Gets and sets the type of calculation in the Totals row of the list column. |
| [range](#range--)| Range | Readonly. Gets the range of this list column. |
| [isArrayFormula](#isArrayFormula--)| boolean | Readonly. Indicates whether the fomula is array formula. |
| [formula](#formula--)| string | Gets and sets the formula of the list column. |
| [totalsRowLabel](#totalsRowLabel--)| string | Gets and sets the display labels of total row. |
## Methods
| Method | Description |
| --- | --- |
| [getName()](#getName--)| <b>@deprecated.</b> Please use the 'name' property instead. Gets and sets the name of the column. |
| [setName(string)](#setName-string-)| <b>@deprecated.</b> Please use the 'name' property instead. Gets and sets the name of the column. |
| [getTotalsCalculation()](#getTotalsCalculation--)| <b>@deprecated.</b> Please use the 'totalsCalculation' property instead. Gets and sets the type of calculation in the Totals row of the list column. |
| [setTotalsCalculation(TotalsCalculation)](#setTotalsCalculation-totalscalculation-)| <b>@deprecated.</b> Please use the 'totalsCalculation' property instead. Gets and sets the type of calculation in the Totals row of the list column. |
| [getRange()](#getRange--)| <b>@deprecated.</b> Please use the 'range' property instead. Gets the range of this list column. |
| [isArrayFormula()](#isArrayFormula--)| <b>@deprecated.</b> Please use the 'isArrayFormula' property instead. Indicates whether the fomula is array formula. |
| [getFormula()](#getFormula--)| <b>@deprecated.</b> Please use the 'formula' property instead. Gets and sets the formula of the list column. |
| [setFormula(string)](#setFormula-string-)| <b>@deprecated.</b> Please use the 'formula' property instead. Gets and sets the formula of the list column. |
| [getTotalsRowLabel()](#getTotalsRowLabel--)| <b>@deprecated.</b> Please use the 'totalsRowLabel' property instead. Gets and sets the display labels of total row. |
| [setTotalsRowLabel(string)](#setTotalsRowLabel-string-)| <b>@deprecated.</b> Please use the 'totalsRowLabel' property instead. Gets and sets the display labels of total row. |
| [getCustomTotalsRowFormula(boolean, boolean)](#getCustomTotalsRowFormula-boolean-boolean-)| Gets the formula of totals row of this list column. |
| [setCustomTotalsRowFormula(string, boolean, boolean)](#setCustomTotalsRowFormula-string-boolean-boolean-)| Gets the formula of totals row of this list column. |
| [getCustomCalculatedFormula(boolean, boolean)](#getCustomCalculatedFormula-boolean-boolean-)| Gets the formula of this list column. |
| [setCustomCalculatedFormula(string, boolean, boolean)](#setCustomCalculatedFormula-string-boolean-boolean-)| Sets the formula for this list column. |
| [getDataStyle()](#getDataStyle--)| Gets the style of the data in this column of the table. |
| [setDataStyle(Style)](#setDataStyle-style-)| Sets the style of the data in this column of the table. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### name {#name--}
Gets and sets the name of the column.
```javascript
name : string;
```
**Remarks**
If sets the name of the column, the according cell' value will be changed too.
### totalsCalculation {#totalsCalculation--}
Gets and sets the type of calculation in the Totals row of the list column.
```javascript
totalsCalculation : TotalsCalculation;
```
### range {#range--}
Readonly. Gets the range of this list column.
```javascript
range : Range;
```
### isArrayFormula {#isArrayFormula--}
Readonly. Indicates whether the fomula is array formula.
```javascript
isArrayFormula : boolean;
```
### formula {#formula--}
Gets and sets the formula of the list column.
```javascript
formula : string;
```
### totalsRowLabel {#totalsRowLabel--}
Gets and sets the display labels of total row.
```javascript
totalsRowLabel : string;
```
### getName() {#getName--}
```javascript
getName() : string;
```
**Remarks**
If sets the name of the column, the according cell' value will be changed too.
### setName(string) {#setName-string-}
```javascript
setName(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
If sets the name of the column, the according cell' value will be changed too.
### getTotalsCalculation() {#getTotalsCalculation--}
```javascript
getTotalsCalculation() : TotalsCalculation;
```
**Returns**
[TotalsCalculation](../totalscalculation/)
### setTotalsCalculation(TotalsCalculation) {#setTotalsCalculation-totalscalculation-}
```javascript
setTotalsCalculation(value: TotalsCalculation) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TotalsCalculation](../totalscalculation/) | The value to set. |
### getRange() {#getRange--}
```javascript
getRange() : Range;
```
**Returns**
[Range](../range/)
### isArrayFormula() {#isArrayFormula--}
```javascript
isArrayFormula() : boolean;
```
### getFormula() {#getFormula--}
```javascript
getFormula() : string;
```
### setFormula(string) {#setFormula-string-}
```javascript
setFormula(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getTotalsRowLabel() {#getTotalsRowLabel--}
```javascript
getTotalsRowLabel() : string;
```
### setTotalsRowLabel(string) {#setTotalsRowLabel-string-}
```javascript
setTotalsRowLabel(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getCustomTotalsRowFormula(boolean, boolean) {#getCustomTotalsRowFormula-boolean-boolean-}
Gets the formula of totals row of this list column.
```javascript
getCustomTotalsRowFormula(isR1C1: boolean, isLocal: boolean) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
**Returns**
The formula of this list column.
### setCustomTotalsRowFormula(string, boolean, boolean) {#setCustomTotalsRowFormula-string-boolean-boolean-}
Gets the formula of totals row of this list column.
```javascript
setCustomTotalsRowFormula(formula: string, isR1C1: boolean, isLocal: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | the formula for this list column. |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
### getCustomCalculatedFormula(boolean, boolean) {#getCustomCalculatedFormula-boolean-boolean-}
Gets the formula of this list column.
```javascript
getCustomCalculatedFormula(isR1C1: boolean, isLocal: boolean) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
**Returns**
The formula of this list column.
### setCustomCalculatedFormula(string, boolean, boolean) {#setCustomCalculatedFormula-string-boolean-boolean-}
Sets the formula for this list column.
```javascript
setCustomCalculatedFormula(formula: string, isR1C1: boolean, isLocal: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | the formula for this list column. |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
### getDataStyle() {#getDataStyle--}
Gets the style of the data in this column of the table.
```javascript
getDataStyle() : Style;
```
**Returns**
[Style](../style/)
### setDataStyle(Style) {#setDataStyle-style-}
Sets the style of the data in this column of the table.
```javascript
setDataStyle(style: Style) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [Style](../style/) |  |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
