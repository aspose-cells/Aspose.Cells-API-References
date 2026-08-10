---
title: "CalculationData Class"
linktitle: "CalculationData"
articleTitle: "CalculationData"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents the required data when calculating one function, such as function name, parameters, ...etc."
type: docs
weight: 490
url: /php/aspose.cells/calculationdata/
---

## CalculationData class

Represents the required data when calculating one function, such as function name, parameters, ...etc.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [CalculatedValue](#calculatedvalue) | Object | Gets or sets the calculated value for this function. User should set this property in his custom calculation engine for  |
| [Workbook](#workbook) | Workbook | Gets the Workbook object where the function is in. |
| [Worksheet](#worksheet) | Worksheet | Gets the Worksheet object where the function is in. |
| [CellRow](#cellrow) | Number | Gets the row index of the cell where the function is in. |
| [CellColumn](#cellcolumn) | Number | Gets the column index of the cell where the function is in. |
| [Cell](#cell) | Cell | Gets the Cell object where the function is in. When calculating a formula without setting it to a cell, such as by Works |
| [FunctionName](#functionname) | String | Gets the function name to be calculated. |
| [ParamCount](#paramcount) | Number | Gets the count of parameters |

## Methods

| Name | Description |
| --- | --- |
| [getParamValue](#getparamvalue) | Gets the represented value object of the parameter at given index.

For one parameter: If it is plain value, then return |
| [getParamValueInArrayMode](#getparamvalueinarraymode) | Gets the value(s) of the parameter at given index. If the parameter is some kind of expression that needs to be calculat |
| [getParamText](#getparamtext) | Gets the literal text of the parameter at given index. |

### CalculationData.CalculatedValue property {#calculatedvalue}

Gets or sets the calculated value for this function. User should set this property in his custom calculation engine for those functions the engine supports, and the set value will be returned when getting this property later. The set value may be of possible types of Cell.Value , or array of such kind of values, or a Range, Name, ReferredArea. Getting this property before setting value to it will make the function be calculated by the default calculation engine of Aspose.Cells and then the calculated value will be returned(generally it should be #NAME? for user-defined functions).

**Type:** Object

### CalculationData.Workbook property {#workbook}

Gets the Workbook object where the function is in.

**Type:** Workbook

### CalculationData.Worksheet property {#worksheet}

Gets the Worksheet object where the function is in.

**Type:** Worksheet

### CalculationData.CellRow property {#cellrow}

Gets the row index of the cell where the function is in.

**Type:** Number

### CalculationData.CellColumn property {#cellcolumn}

Gets the column index of the cell where the function is in.

**Type:** Number

### CalculationData.Cell property {#cell}

Gets the Cell object where the function is in. When calculating a formula without setting it to a cell, such as by Worksheet.calculateFormula(java.lang.String, com.aspose.cells.CalculationOptions) , the formula will be calculated just like it has been set to cell A1, so both CellRow and CellColumn are 0. However, cell A1 in the worksheet may has not been instantiated. So for such kind of situation this property will be null.

**Type:** Cell

### CalculationData.FunctionName property {#functionname}

Gets the function name to be calculated.

**Type:** String

### CalculationData.ParamCount property {#paramcount}

Gets the count of parameters

**Type:** Number

### getParamValue(index) {#getparamvalue}

Gets the represented value object of the parameter at given index.

For one parameter: If it is plain value, then returns the plain value itself; If it is reference, then returns ReferredArea object; If it references to dataset(s) with multiple values, then returns array of objects; If it is some kind of expression that needs to be calculated, then it will be calculated in value mode and generally a single value will be returned according to current cell base. For example, if one parameter of D2's formula is A:A+B:B, then A2+B2 will be calculated and returned. However, if this parameter has been specified as array mode (by Workbook.updateCustomFunctionDefinition(com.aspose.cells.CustomFunctionDefinition) or FormulaParseOptions.CustomFunctionDefinition ), then an array(object[][]) will be returned whose items are A1+B1,A2+B2,....

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index of the parameter(0 based) |

**Returns:** The calculated value of the parameter.

### getParamValueInArrayMode(index, maxRowCount, maxColumnCount) {#getparamvalueinarraymode}

Gets the value(s) of the parameter at given index. If the parameter is some kind of expression that needs to be calculated, then it will be calculated in array mode.

For an expression that needs to be calculated, taking A:A+B:B as an example: In value mode it will be calculated to a single value according to current cell base. But in array mode, all values of A1+B1,A2+B2,A3+B3,... will be calculated and used to construct the returned array. And for such kind of situation, it is better to specify the limit for the row/column count (such as according to Cells.MaxDataRow and Cells.MaxDataColumn ), otherwise the returned large array may increase memory cost with large amount of useless data.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | The index of the parameter(0 based) |
| maxRowCount | Number | The row count limit for the returned array. If it is non-positive or greater than the actual row count, then actual row count will be used. |
| maxColumnCount | Number | The column count limit for the returned array. If it is non-positive or greater than the actual row count, then actual column count will be used. |

**Returns:** An array which contains all items represented by the specified parameter.

### getParamText(index) {#getparamtext}

Gets the literal text of the parameter at given index.

| Parameter | Type | Description |
| --- | --- | --- |
| index | Number | index of the parameter(0 based) |

**Returns:** literal text of the parameter
