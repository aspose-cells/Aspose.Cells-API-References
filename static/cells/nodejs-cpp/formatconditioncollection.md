##FormatConditionCollection
Represents conditional formatting. The FormatConditions can contain up to three conditional formats.
## FormatConditionCollection class
Represents conditional formatting. The FormatConditions can contain up to three conditional formats.
```javascript
class FormatConditionCollection;
```
### Example
```javascript
const { Workbook, CellArea, FormatConditionType, OperatorType, Color } = require("aspose.cells.node");
//Adds an empty conditional formatting
var workbook = new Workbook();
var sheet = workbook.worksheets.get(0);
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
workbook.save("output/FormatConditionCollection.xls");
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [count](#count--)| number | Readonly. Gets the count of the conditions. |
| [rangeCount](#rangeCount--)| number | Readonly. Gets count of conditionally formatted ranges. |
## Methods
| Method | Description |
| --- | --- |
| [get(number)](#get-number-)| Gets the formatting condition by index. |
| [getCount()](#getCount--)| <b>@deprecated.</b> Please use the 'count' property instead. Gets the count of the conditions. |
| [getRangeCount()](#getRangeCount--)| <b>@deprecated.</b> Please use the 'rangeCount' property instead. Gets count of conditionally formatted ranges. |
| [add(CellArea, FormatConditionType, OperatorType, string, string)](#add-cellarea-formatconditiontype-operatortype-string-string-)| Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats. References to the other sheets are not allowed in the formulas of conditional formatting. |
| [addArea(CellArea)](#addArea-cellarea-)| Adds a conditional formatted cell range. |
| [addCondition(FormatConditionType, OperatorType, string, string)](#addCondition-formatconditiontype-operatortype-string-string-)| Adds a formatting condition. |
| [addCondition(FormatConditionType)](#addCondition-formatconditiontype-)| Add a format condition. |
| [getCellArea(number)](#getCellArea-number-)| Gets the conditional formatted cell range by index. |
| [removeArea(number)](#removeArea-number-)| Removes conditional formatted cell range by index. |
| [removeArea(number, number, number, number)](#removeArea-number-number-number-number-)| Remove conditional formatting int the range. |
| [removeCondition(number)](#removeCondition-number-)| Removes the formatting condition by index. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### count {#count--}
Readonly. Gets the count of the conditions.
```javascript
count : number;
```
### rangeCount {#rangeCount--}
Readonly. Gets count of conditionally formatted ranges.
```javascript
rangeCount : number;
```
### get(number) {#get-number-}
Gets the formatting condition by index.
```javascript
get(index: number) : FormatCondition;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | the index of the formatting condition to return. |
**Returns**
the formatting condition
### getCount() {#getCount--}
```javascript
getCount() : number;
```
### getRangeCount() {#getRangeCount--}
```javascript
getRangeCount() : number;
```
### add(CellArea, FormatConditionType, OperatorType, string, string) {#add-cellarea-formatconditiontype-operatortype-string-string-}
Adds a formatting condition and effected cell rang to the FormatConditions The FormatConditions can contain up to three conditional formats. References to the other sheets are not allowed in the formulas of conditional formatting.
```javascript
add(cellArea: CellArea, type: FormatConditionType, operatorType: OperatorType, formula1: string, formula2: string) : number[];
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../cellarea/) | Conditional formatted cell range. |
| type | [FormatConditionType](../formatconditiontype/) | Type of conditional formatting.It could be one of the members of FormatConditionType. |
| operatorType | [OperatorType](../operatortype/) | Comparison operator.It could be one of the members of OperatorType. |
| formula1 | string | The value or expression associated with conditional formatting. |
| formula2 | string | The value or expression associated with conditional formatting |
**Returns**
[0]:Formatting condition object index;[1] Effected cell rang index.
### addArea(CellArea) {#addArea-cellarea-}
Adds a conditional formatted cell range.
```javascript
addArea(cellArea: CellArea) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../cellarea/) | Conditional formatted cell range. |
**Returns**
Conditional formatted cell rang index.
### addCondition(FormatConditionType, OperatorType, string, string) {#addCondition-formatconditiontype-operatortype-string-string-}
Adds a formatting condition.
```javascript
addCondition(type: FormatConditionType, operatorType: OperatorType, formula1: string, formula2: string) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [FormatConditionType](../formatconditiontype/) | The type of format condition. |
| operatorType | [OperatorType](../operatortype/) | The operator type |
| formula1 | string | The value or expression associated with conditional formatting.         /// If the input value starts with '=', then it will be taken as formula.         /// Otherwise it will be taken as plain value(text, number, bool).         /// For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| formula2 | string | The value or expression associated with conditional formatting.         /// The input format is same with formula1 |
**Returns**
Formatting condition object index;
### addCondition(FormatConditionType) {#addCondition-formatconditiontype-}
Add a format condition.
```javascript
addCondition(type: FormatConditionType) : number;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| type | [FormatConditionType](../formatconditiontype/) | Format condition type. |
**Returns**
Formatting condition object index;
### getCellArea(number) {#getCellArea-number-}
Gets the conditional formatted cell range by index.
```javascript
getCellArea(index: number) : CellArea;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | the index of the conditional formatted cell range. |
**Returns**
the conditional formatted cell range
### removeArea(number) {#removeArea-number-}
Removes conditional formatted cell range by index.
```javascript
removeArea(index: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index of the conditional formatted cell range to be removed. |
### removeArea(number, number, number, number) {#removeArea-number-number-number-number-}
Remove conditional formatting int the range.
```javascript
removeArea(startRow: number, startColumn: number, totalRows: number, totalColumns: number) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | number | The startRow of the range. |
| startColumn | number | The startColumn of the range. |
| totalRows | number | The number of rows of the range. |
| totalColumns | number | The number of columns of the range. |
**Returns**
Returns TRUE, this FormatCondtionCollection should be removed.
### removeCondition(number) {#removeCondition-number-}
Removes the formatting condition by index.
```javascript
removeCondition(index: number) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index of the formatting condition to be removed. |
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
