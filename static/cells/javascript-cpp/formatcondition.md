##FormatCondition
Represents conditional formatting condition.
## FormatCondition class
Represents conditional formatting condition.
```javascript
class FormatCondition;
```
### Example
```javascript
const { Workbook, CellArea, FormatConditionType, OperatorType, Color, SaveFormat } = AsposeCells;
//Instantiating a Workbook object
var workbook = new Workbook();
var sheet = workbook.worksheets.get(0);
//Adds an empty conditional formatting
var index = sheet.conditionalFormattings.add();
var fcs = sheet.conditionalFormattings.get(index);
//Sets the conditional format range.
var ca = new CellArea();
ca.startRow = 0;
ca.endRow = 0;
ca.startColumn = 0;
ca.endColumn = 0;
fcs.addArea(ca);
ca = new CellArea();
ca.startRow = 1;
ca.endRow = 1;
ca.startColumn = 1;
ca.endColumn = 1;
fcs.addArea(ca);
//Adds condition.
var conditionIndex = fcs.addCondition(FormatConditionType.CellValue, OperatorType.Between, "=A2", "100");
//Adds condition.
var conditionIndex2 = fcs.addCondition(FormatConditionType.CellValue, OperatorType.Between, "50", "100");
//Sets the background color.
var fc = fcs.get(conditionIndex);
fc.style.backgroundColor = Color.Red;
//Saving the Excel file
var uint8Array = workbook.save(SaveFormat.Xlsx);
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [formula1](#formula1--)| string | Gets and sets the value or expression associated with conditional formatting. |
| [formula2](#formula2--)| string | Gets and sets the value or expression associated with conditional formatting. |
| [operator](#operator--)| OperatorType | Gets and sets the conditional format operator type. |
| [stopIfTrue](#stopIfTrue--)| boolean | True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. Only applies for Excel 2007; |
| [priority](#priority--)| number | The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values, where '1' is the highest priority. |
| [style](#style--)| Style | Gets or setts style of conditional formatted cell ranges. |
| [type](#type--)| FormatConditionType | Gets and sets whether the conditional format Type. |
| [iconSet](#iconSet--)| IconSet | Readonly. Get the conditional formatting's "IconSet" instance. The default instance's IconSetType is TrafficLights31. Valid only for type = IconSet. |
| [dataBar](#dataBar--)| DataBar | Readonly. Get the conditional formatting's "DataBar" instance. The default instance's color is blue. Valid only for type is DataBar. |
| [colorScale](#colorScale--)| ColorScale | Readonly. Get the conditional formatting's "ColorScale" instance. The default instance is a "green-yellow-red" 3ColorScale . Valid only for type = ColorScale. |
| [top10](#top10--)| Top10 | Readonly. Get the conditional formatting's "Top10" instance. The default instance's rule highlights cells whose values fall in the top 10 bracket. Valid only for type is Top10. |
| [aboveAverage](#aboveAverage--)| AboveAverage | Readonly. Get the conditional formatting's "AboveAverage" instance. The default instance's rule highlights cells that are above the average for all values in the range. Valid only for type = AboveAverage. |
| [text](#text--)| string | The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, beginsWith and endsWith. The default value is null. |
| [timePeriod](#timePeriod--)| TimePeriodType | The applicable time period in a "date occurring…" conditional formatting rule. Valid only for type = timePeriod. The default value is TimePeriodType.Today. |
## Methods
| Method | Description |
| --- | --- |
| [getFormula1(boolean, boolean)](#getFormula1-boolean-boolean-)| Gets the value or expression associated with this format condition. |
| [getFormula1(boolean, boolean, number, number)](#getFormula1-boolean-boolean-number-number-)| Gets the value or expression of the conditional formatting of the cell. |
| [getFormula1(number, number)](#getFormula1-number-number-)| Gets the formula of the conditional formatting of the cell. |
| [getFormula2(boolean, boolean)](#getFormula2-boolean-boolean-)| Gets the value or expression associated with this format condition. |
| [getFormula2(boolean, boolean, number, number)](#getFormula2-boolean-boolean-number-number-)| Gets the value or expression of the conditional formatting of the cell. |
| [getFormula2(number, number)](#getFormula2-number-number-)| Gets the formula of the conditional formatting of the cell. |
| [setFormulas(string, string, boolean, boolean)](#setFormulas-string-string-boolean-boolean-)| Sets the value or expression associated with this format condition. |
| [setFormula1(string, boolean, boolean)](#setFormula1-string-boolean-boolean-)| Sets the value or expression associated with this format condition. |
| [setFormula2(string, boolean, boolean)](#setFormula2-string-boolean-boolean-)| Sets the value or expression associated with this format condition. |
### formula1 {#formula1--}
Gets and sets the value or expression associated with conditional formatting.
```javascript
formula1 : string;
```
**Remarks**
Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"".
### formula2 {#formula2--}
Gets and sets the value or expression associated with conditional formatting.
```javascript
formula2 : string;
```
**Remarks**
Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"".
### operator {#operator--}
Gets and sets the conditional format operator type.
```javascript
operator : OperatorType;
```
### stopIfTrue {#stopIfTrue--}
True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. Only applies for Excel 2007;
```javascript
stopIfTrue : boolean;
```
### priority {#priority--}
The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values, where '1' is the highest priority.
```javascript
priority : number;
```
### style {#style--}
Gets or setts style of conditional formatted cell ranges.
```javascript
style : Style;
```
### type {#type--}
Gets and sets whether the conditional format Type.
```javascript
type : FormatConditionType;
```
### iconSet {#iconSet--}
Readonly. Get the conditional formatting's "IconSet" instance. The default instance's IconSetType is TrafficLights31. Valid only for type = IconSet.
```javascript
iconSet : IconSet;
```
### dataBar {#dataBar--}
Readonly. Get the conditional formatting's "DataBar" instance. The default instance's color is blue. Valid only for type is DataBar.
```javascript
dataBar : DataBar;
```
### colorScale {#colorScale--}
Readonly. Get the conditional formatting's "ColorScale" instance. The default instance is a "green-yellow-red" 3ColorScale . Valid only for type = ColorScale.
```javascript
colorScale : ColorScale;
```
### top10 {#top10--}
Readonly. Get the conditional formatting's "Top10" instance. The default instance's rule highlights cells whose values fall in the top 10 bracket. Valid only for type is Top10.
```javascript
top10 : Top10;
```
### aboveAverage {#aboveAverage--}
Readonly. Get the conditional formatting's "AboveAverage" instance. The default instance's rule highlights cells that are above the average for all values in the range. Valid only for type = AboveAverage.
```javascript
aboveAverage : AboveAverage;
```
### text {#text--}
The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, beginsWith and endsWith. The default value is null.
```javascript
text : string;
```
### timePeriod {#timePeriod--}
The applicable time period in a "date occurring…" conditional formatting rule. Valid only for type = timePeriod. The default value is TimePeriodType.Today.
```javascript
timePeriod : TimePeriodType;
```
### getFormula1(boolean, boolean) {#getFormula1-boolean-boolean-}
Gets the value or expression associated with this format condition.
```javascript
getFormula1(isR1C1: boolean, isLocal: boolean) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
**Returns**
The value or expression associated with this format condition.
### getFormula1(boolean, boolean, number, number) {#getFormula1-boolean-boolean-number-number-}
Gets the value or expression of the conditional formatting of the cell.
```javascript
getFormula1(isR1C1: boolean, isLocal: boolean, row: number, column: number) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
| row | number | The row index. |
| column | number | The column index. |
**Returns**
The value or expression associated with the conditional formatting of the cell.
**Remarks**
The given cell must be contained by this conditional formatting, otherwise null will be returned.
### getFormula1(number, number) {#getFormula1-number-number-}
Gets the formula of the conditional formatting of the cell.
```javascript
getFormula1(row: number, column: number) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index. |
| column | number | The column index. |
**Returns**
The formula.
### getFormula2(boolean, boolean) {#getFormula2-boolean-boolean-}
Gets the value or expression associated with this format condition.
```javascript
getFormula2(isR1C1: boolean, isLocal: boolean) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
**Returns**
The value or expression associated with this format condition.
### getFormula2(boolean, boolean, number, number) {#getFormula2-boolean-boolean-number-number-}
Gets the value or expression of the conditional formatting of the cell.
```javascript
getFormula2(isR1C1: boolean, isLocal: boolean, row: number, column: number) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
| row | number | The row index. |
| column | number | The column index. |
**Returns**
The value or expression associated with the conditional formatting of the cell.
**Remarks**
The given cell must be contained by this conditional formatting, otherwise null will be returned.
### getFormula2(number, number) {#getFormula2-number-number-}
Gets the formula of the conditional formatting of the cell.
```javascript
getFormula2(row: number, column: number) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | number | The row index. |
| column | number | The column index. |
**Returns**
The formula.
### setFormulas(string, string, boolean, boolean) {#setFormulas-string-string-boolean-boolean-}
Sets the value or expression associated with this format condition.
```javascript
setFormulas(formula1: string, formula2: string, isR1C1: boolean, isLocal: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula1 | string | The value or expression associated with this format condition.         /// If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool).         /// For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| formula2 | string | The value or expression associated with this format condition. The input format is same with formula1 |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |
### setFormula1(string, boolean, boolean) {#setFormula1-string-boolean-boolean-}
Sets the value or expression associated with this format condition.
```javascript
setFormula1(formula: string, isR1C1: boolean, isLocal: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | The value or expression associated with this format condition.         /// If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool).         /// For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |
### setFormula2(string, boolean, boolean) {#setFormula2-string-boolean-boolean-}
Sets the value or expression associated with this format condition.
```javascript
setFormula2(formula: string, isR1C1: boolean, isLocal: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | string | The value or expression associated with this format condition.         /// If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool).         /// For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |
