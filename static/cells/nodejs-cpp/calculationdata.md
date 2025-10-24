##CalculationData
Represents the required data when calculating one function such as function name parameters ...etc.
## CalculationData class
Represents the required data when calculating one function, such as function name, parameters, ...etc.
```javascript
class CalculationData;
```
### Remarks
All objects provided by this class are for "read" purpose only. User should not change any data in the Workbook during the formula calculation process, Otherwise unexpected result or Exception may be caused.
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [calculatedValue](#calculatedValue--)| Object | Gets or sets the calculated value for this function. |
| [workbook](#workbook--)| Workbook | Readonly. Gets the Workbook object where the function is in. |
| [worksheet](#worksheet--)| Worksheet | Readonly. Gets the Worksheet object where the function is in. |
| [cellRow](#cellRow--)| number | Readonly. Gets the row index of the cell where the function is in. |
| [cellColumn](#cellColumn--)| number | Readonly. Gets the column index of the cell where the function is in. |
| [cell](#cell--)| Cell | Readonly. Gets the Cell object where the function is in. |
| [functionName](#functionName--)| string | Readonly. Gets the function name to be calculated. |
| [paramCount](#paramCount--)| number | Readonly. Gets the count of parameters |
## Methods
| Method | Description |
| --- | --- |
| [getCalculatedValue()](#getCalculatedValue--)| <b>@deprecated.</b> Please use the 'calculatedValue' property instead. Gets or sets the calculated value for this function. |
| [setCalculatedValue(Object)](#setCalculatedValue-object-)| <b>@deprecated.</b> Please use the 'calculatedValue' property instead. Gets or sets the calculated value for this function. |
| [getWorkbook()](#getWorkbook--)| <b>@deprecated.</b> Please use the 'workbook' property instead. Gets the Workbook object where the function is in. |
| [getWorksheet()](#getWorksheet--)| <b>@deprecated.</b> Please use the 'worksheet' property instead. Gets the Worksheet object where the function is in. |
| [getCellRow()](#getCellRow--)| <b>@deprecated.</b> Please use the 'cellRow' property instead. Gets the row index of the cell where the function is in. |
| [getCellColumn()](#getCellColumn--)| <b>@deprecated.</b> Please use the 'cellColumn' property instead. Gets the column index of the cell where the function is in. |
| [getCell()](#getCell--)| <b>@deprecated.</b> Please use the 'cell' property instead. Gets the Cell object where the function is in. |
| [getFunctionName()](#getFunctionName--)| <b>@deprecated.</b> Please use the 'functionName' property instead. Gets the function name to be calculated. |
| [getParamCount()](#getParamCount--)| <b>@deprecated.</b> Please use the 'paramCount' property instead. Gets the count of parameters |
| [getParamValue(number)](#getParamValue-number-)| Gets the represented value object of the parameter at given index. |
| [getParamValueInArrayMode(number, number, number)](#getParamValueInArrayMode-number-number-number-)| Gets the value(s) of the parameter at given index. If the parameter is some kind of expression that needs to be calculated, then it will be calculated in array mode. |
| [getParamText(number)](#getParamText-number-)| Gets the literal text of the parameter at given index. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### calculatedValue {#calculatedValue--}
Gets or sets the calculated value for this function.
```javascript
calculatedValue : Object;
```
**Remarks**
User should set this property in his custom calculation engine for those functions the engine supports, and the set value will be returned when getting this property later. The set value may be of possible types of [Cell.Value](../cell.value/), or array of such kind of values, or a Range, Name, ReferredArea. Getting this property before setting value to it will make the function be calculated by the default calculation engine of Aspose.Cells and then the calculated value will be returned(generally it should be #NAME? for user-defined functions).
### workbook {#workbook--}
Readonly. Gets the Workbook object where the function is in.
```javascript
workbook : Workbook;
```
### worksheet {#worksheet--}
Readonly. Gets the Worksheet object where the function is in.
```javascript
worksheet : Worksheet;
```
### cellRow {#cellRow--}
Readonly. Gets the row index of the cell where the function is in.
```javascript
cellRow : number;
```
### cellColumn {#cellColumn--}
Readonly. Gets the column index of the cell where the function is in.
```javascript
cellColumn : number;
```
### cell {#cell--}
Readonly. Gets the Cell object where the function is in.
```javascript
cell : Cell;
```
**Remarks**
When calculating a formula without setting it to a cell, such as by [Worksheet.CalculateFormula(string, CalculationOptions)](../worksheet.calculateformula(string, calculationoptions)/), the formula will be calculated just like it has been set to cell A1, so both [CellRow](../cellrow/) and [CellColumn](../cellcolumn/) are 0. However, cell A1 in the worksheet may has not been instantiated. So for such kind of situation this property will be null.
### functionName {#functionName--}
Readonly. Gets the function name to be calculated.
```javascript
functionName : string;
```
### paramCount {#paramCount--}
Readonly. Gets the count of parameters
```javascript
paramCount : number;
```
### getCalculatedValue() {#getCalculatedValue--}
```javascript
getCalculatedValue() : Object;
```
**Remarks**
User should set this property in his custom calculation engine for those functions the engine supports, and the set value will be returned when getting this property later. The set value may be of possible types of [Cell.Value](../cell.value/), or array of such kind of values, or a Range, Name, ReferredArea. Getting this property before setting value to it will make the function be calculated by the default calculation engine of Aspose.Cells and then the calculated value will be returned(generally it should be #NAME? for user-defined functions).
### setCalculatedValue(Object) {#setCalculatedValue-object-}
```javascript
setCalculatedValue(value: Object) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | Object | The value to set. |
**Remarks**
User should set this property in his custom calculation engine for those functions the engine supports, and the set value will be returned when getting this property later. The set value may be of possible types of [Cell.Value](../cell.value/), or array of such kind of values, or a Range, Name, ReferredArea. Getting this property before setting value to it will make the function be calculated by the default calculation engine of Aspose.Cells and then the calculated value will be returned(generally it should be #NAME? for user-defined functions).
### getWorkbook() {#getWorkbook--}
```javascript
getWorkbook() : Workbook;
```
**Returns**
[Workbook](../workbook/)
### getWorksheet() {#getWorksheet--}
```javascript
getWorksheet() : Worksheet;
```
**Returns**
[Worksheet](../worksheet/)
### getCellRow() {#getCellRow--}
```javascript
getCellRow() : number;
```
### getCellColumn() {#getCellColumn--}
```javascript
getCellColumn() : number;
```
### getCell() {#getCell--}
```javascript
getCell() : Cell;
```
**Returns**
[Cell](../cell/)
**Remarks**
When calculating a formula without setting it to a cell, such as by [Worksheet.CalculateFormula(string, CalculationOptions)](../worksheet.calculateformula(string, calculationoptions)/), the formula will be calculated just like it has been set to cell A1, so both [CellRow](../cellrow/) and [CellColumn](../cellcolumn/) are 0. However, cell A1 in the worksheet may has not been instantiated. So for such kind of situation this property will be null.
### getFunctionName() {#getFunctionName--}
```javascript
getFunctionName() : string;
```
### getParamCount() {#getParamCount--}
```javascript
getParamCount() : number;
```
### getParamValue(number) {#getParamValue-number-}
Gets the represented value object of the parameter at given index.
```javascript
getParamValue(index: number) : Object;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index of the parameter(0 based) |
**Returns**
The calculated value of the parameter.
**Remarks**
For one parameter: <p>If it is plain value, then returns the plain value itself;</p> <p>If it is reference, then returns ReferredArea object;</p> <p>If it references to dataset(s) with multiple values, then returns array of objects;</p> <p> If it is some kind of expression that needs to be calculated, then it will be calculated in value mode and generally a single value will be returned according to current cell base. For example, if one parameter of D2's formula is A:A+B:B, then A2+B2 will be calculated and returned. However, if this parameter has been specified as array mode (by [Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)](../workbook.updatecustomfunctiondefinition(customfunctiondefinition)/) or [FormulaParseOptions.CustomFunctionDefinition](../formulaparseoptions.customfunctiondefinition/)), then an array(object[][]) will be returned whose items are A1+B1,A2+B2,....
### getParamValueInArrayMode(number, number, number) {#getParamValueInArrayMode-number-number-number-}
Gets the value(s) of the parameter at given index. If the parameter is some kind of expression that needs to be calculated, then it will be calculated in array mode.
```javascript
getParamValueInArrayMode(index: number, maxRowCount: number, maxColumnCount: number) : Object[][];
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | The index of the parameter(0 based) |
| maxRowCount | number | The row count limit for the returned array.         /// If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | number | The column count limit for the returned array.         /// If it is non-positive or greater than the actual row count, then actual column count will be used. |
**Returns**
An array which contains all items represented by the specified parameter.
**Remarks**
For an expression that needs to be calculated, taking A:A+B:B as an example: In value mode it will be calculated to a single value according to current cell base. But in array mode, all values of A1+B1,A2+B2,A3+B3,... will be calculated and used to construct the returned array. And for such kind of situation, it is better to specify the limit for the row/column count (such as according to [Cells.MaxDataRow](../cells.maxdatarow/) and [Cells.MaxDataColumn](../cells.maxdatacolumn/)), otherwise the returned large array may increase memory cost with large amount of useless data.
### getParamText(number) {#getParamText-number-}
Gets the literal text of the parameter at given index.
```javascript
getParamText(index: number) : string;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | number | index of the parameter(0 based) |
**Returns**
literal text of the parameter
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
