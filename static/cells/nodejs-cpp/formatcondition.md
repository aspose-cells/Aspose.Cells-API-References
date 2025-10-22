##FormatCondition
Represents conditional formatting condition.
## FormatCondition class
Represents conditional formatting condition.
```javascript
class FormatCondition;
```
### Example
```javascript
const { Workbook, CellArea, FormatConditionType, OperatorType, Color } = require("aspose.cells.node");
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
workbook.save("output/FormatCondition.xls");
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
| [getFormula1()](#getFormula1--)| <b>@deprecated.</b> Please use the 'formula1' property instead. Gets and sets the value or expression associated with conditional formatting. |
| [setFormula1(string)](#setFormula1-string-)| <b>@deprecated.</b> Please use the 'formula1' property instead. Gets and sets the value or expression associated with conditional formatting. |
| [getFormula2()](#getFormula2--)| <b>@deprecated.</b> Please use the 'formula2' property instead. Gets and sets the value or expression associated with conditional formatting. |
| [setFormula2(string)](#setFormula2-string-)| <b>@deprecated.</b> Please use the 'formula2' property instead. Gets and sets the value or expression associated with conditional formatting. |
| [getOperator()](#getOperator--)| <b>@deprecated.</b> Please use the 'operator' property instead. Gets and sets the conditional format operator type. |
| [setOperator(OperatorType)](#setOperator-operatortype-)| <b>@deprecated.</b> Please use the 'operator' property instead. Gets and sets the conditional format operator type. |
| [getStopIfTrue()](#getStopIfTrue--)| <b>@deprecated.</b> Please use the 'stopIfTrue' property instead. True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. Only applies for Excel 2007; |
| [setStopIfTrue(boolean)](#setStopIfTrue-boolean-)| <b>@deprecated.</b> Please use the 'stopIfTrue' property instead. True, no rules with lower priority may be applied over this rule, when this rule evaluates to true. Only applies for Excel 2007; |
| [getPriority()](#getPriority--)| <b>@deprecated.</b> Please use the 'priority' property instead. The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values, where '1' is the highest priority. |
| [setPriority(number)](#setPriority-number-)| <b>@deprecated.</b> Please use the 'priority' property instead. The priority of this conditional formatting rule. This value is used to determine which format should be evaluated and rendered. Lower numeric values are higher priority than higher numeric values, where '1' is the highest priority. |
| [getStyle()](#getStyle--)| <b>@deprecated.</b> Please use the 'style' property instead. Gets or setts style of conditional formatted cell ranges. |
| [setStyle(Style)](#setStyle-style-)| <b>@deprecated.</b> Please use the 'style' property instead. Gets or setts style of conditional formatted cell ranges. |
| [getType()](#getType--)| <b>@deprecated.</b> Please use the 'type' property instead. Gets and sets whether the conditional format Type. |
| [setType(FormatConditionType)](#setType-formatconditiontype-)| <b>@deprecated.</b> Please use the 'type' property instead. Gets and sets whether the conditional format Type. |
| [getIconSet()](#getIconSet--)| <b>@deprecated.</b> Please use the 'iconSet' property instead. Get the conditional formatting's "IconSet" instance. The default instance's IconSetType is TrafficLights31. Valid only for type = IconSet. |
| [getDataBar()](#getDataBar--)| <b>@deprecated.</b> Please use the 'dataBar' property instead. Get the conditional formatting's "DataBar" instance. The default instance's color is blue. Valid only for type is DataBar. |
| [getColorScale()](#getColorScale--)| <b>@deprecated.</b> Please use the 'colorScale' property instead. Get the conditional formatting's "ColorScale" instance. The default instance is a "green-yellow-red" 3ColorScale . Valid only for type = ColorScale. |
| [getTop10()](#getTop10--)| <b>@deprecated.</b> Please use the 'top10' property instead. Get the conditional formatting's "Top10" instance. The default instance's rule highlights cells whose values fall in the top 10 bracket. Valid only for type is Top10. |
| [getAboveAverage()](#getAboveAverage--)| <b>@deprecated.</b> Please use the 'aboveAverage' property instead. Get the conditional formatting's "AboveAverage" instance. The default instance's rule highlights cells that are above the average for all values in the range. Valid only for type = AboveAverage. |
| [getText()](#getText--)| <b>@deprecated.</b> Please use the 'text' property instead. The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, beginsWith and endsWith. The default value is null. |
| [setText(string)](#setText-string-)| <b>@deprecated.</b> Please use the 'text' property instead. The text value in a "text contains" conditional formatting rule. Valid only for type = containsText, notContainsText, beginsWith and endsWith. The default value is null. |
| [getTimePeriod()](#getTimePeriod--)| <b>@deprecated.</b> Please use the 'timePeriod' property instead. The applicable time period in a "date occurring…" conditional formatting rule. Valid only for type = timePeriod. The default value is TimePeriodType.Today. |
| [setTimePeriod(TimePeriodType)](#setTimePeriod-timeperiodtype-)| <b>@deprecated.</b> Please use the 'timePeriod' property instead. The applicable time period in a "date occurring…" conditional formatting rule. Valid only for type = timePeriod. The default value is TimePeriodType.Today. |
| [getFormula1(boolean, boolean)](#getFormula1-boolean-boolean-)| Gets the value or expression associated with this format condition. |
| [getFormula1(boolean, boolean, number, number)](#getFormula1-boolean-boolean-number-number-)| Gets the value or expression of the conditional formatting of the cell. |
| [getFormula1(number, number)](#getFormula1-number-number-)| Gets the formula of the conditional formatting of the cell. |
| [getFormula2(boolean, boolean)](#getFormula2-boolean-boolean-)| Gets the value or expression associated with this format condition. |
| [getFormula2(boolean, boolean, number, number)](#getFormula2-boolean-boolean-number-number-)| Gets the value or expression of the conditional formatting of the cell. |
| [getFormula2(number, number)](#getFormula2-number-number-)| Gets the formula of the conditional formatting of the cell. |
| [setFormulas(string, string, boolean, boolean)](#setFormulas-string-string-boolean-boolean-)| Sets the value or expression associated with this format condition. |
| [setFormula1(string, boolean, boolean)](#setFormula1-string-boolean-boolean-)| Sets the value or expression associated with this format condition. |
| [setFormula2(string, boolean, boolean)](#setFormula2-string-boolean-boolean-)| Sets the value or expression associated with this format condition. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
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
### getFormula1() {#getFormula1--}
```javascript
getFormula1() : string;
```
**Remarks**
Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"".
### setFormula1(string) {#setFormula1-string-}
```javascript
setFormula1(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"".
### getFormula2() {#getFormula2--}
```javascript
getFormula2() : string;
```
**Remarks**
Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"".
### setFormula2(string) {#setFormula2-string-}
```javascript
setFormula2(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
Please add all areas before setting formula. For setting formula for this condition, if the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool). For text value that starts with '=', user may input it as formula in format: "=\"=...\"".
### getOperator() {#getOperator--}
```javascript
getOperator() : OperatorType;
```
**Returns**
[OperatorType](../operatortype/)
### setOperator(OperatorType) {#setOperator-operatortype-}
```javascript
setOperator(value: OperatorType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [OperatorType](../operatortype/) | The value to set. |
### getStopIfTrue() {#getStopIfTrue--}
```javascript
getStopIfTrue() : boolean;
```
### setStopIfTrue(boolean) {#setStopIfTrue-boolean-}
```javascript
setStopIfTrue(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getPriority() {#getPriority--}
```javascript
getPriority() : number;
```
### setPriority(number) {#setPriority-number-}
```javascript
setPriority(value: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | number | The value to set. |
### getStyle() {#getStyle--}
```javascript
getStyle() : Style;
```
**Returns**
[Style](../style/)
### setStyle(Style) {#setStyle-style-}
```javascript
setStyle(value: Style) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Style](../style/) | The value to set. |
### getType() {#getType--}
```javascript
getType() : FormatConditionType;
```
**Returns**
[FormatConditionType](../formatconditiontype/)
### setType(FormatConditionType) {#setType-formatconditiontype-}
```javascript
setType(value: FormatConditionType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [FormatConditionType](../formatconditiontype/) | The value to set. |
### getIconSet() {#getIconSet--}
```javascript
getIconSet() : IconSet;
```
**Returns**
[IconSet](../iconset/)
### getDataBar() {#getDataBar--}
```javascript
getDataBar() : DataBar;
```
**Returns**
[DataBar](../databar/)
### getColorScale() {#getColorScale--}
```javascript
getColorScale() : ColorScale;
```
**Returns**
[ColorScale](../colorscale/)
### getTop10() {#getTop10--}
```javascript
getTop10() : Top10;
```
**Returns**
[Top10](../top10/)
### getAboveAverage() {#getAboveAverage--}
```javascript
getAboveAverage() : AboveAverage;
```
**Returns**
[AboveAverage](../aboveaverage/)
### getText() {#getText--}
```javascript
getText() : string;
```
### setText(string) {#setText-string-}
```javascript
setText(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
### getTimePeriod() {#getTimePeriod--}
```javascript
getTimePeriod() : TimePeriodType;
```
**Returns**
[TimePeriodType](../timeperiodtype/)
### setTimePeriod(TimePeriodType) {#setTimePeriod-timeperiodtype-}
```javascript
setTimePeriod(value: TimePeriodType) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [TimePeriodType](../timeperiodtype/) | The value to set. |
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
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
