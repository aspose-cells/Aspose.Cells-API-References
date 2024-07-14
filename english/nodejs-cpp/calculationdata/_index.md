---
title: CalculationData
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the required data when calculating one function such as function name parameters ...etc.
type: docs
url: /nodejs-cpp/calculationdata/
---

## CalculationData class

Represents the required data when calculating one function, such as function name, parameters, ...etc.

```javascript
class CalculationData;
```

### Remarks
All objects provided by this class are for "read" purpose only. User should not change any data in the Workbook during the formula calculation process, Otherwise unexpected result or Exception may be caused.

## Methods

| Method | Description |
| --- | --- |
| [getWorkbook()](#getWorkbook--)| Gets the Workbook object where the function is in. |
| [getWorksheet()](#getWorksheet--)| Gets the Worksheet object where the function is in. |
| [getCellRow()](#getCellRow--)| Gets the row index of the cell where the function is in. |
| [getCellColumn()](#getCellColumn--)| Gets the column index of the cell where the function is in. |
| [getCell()](#getCell--)| Gets the Cell object where the function is in. |
| [getFunctionName()](#getFunctionName--)| Gets the function name to be calculated. |
| [getParamCount()](#getParamCount--)| Gets the count of parameters |
| [getParamText(number)](#getParamText-number-)| Gets the literal text of the parameter at given index. |


### getWorkbook() {#getWorkbook--}

Gets the Workbook object where the function is in.

```javascript
getWorkbook() : Workbook;
```


**Returns**

[Workbook](/nodejs-cpp/workbook/)

### getWorksheet() {#getWorksheet--}

Gets the Worksheet object where the function is in.

```javascript
getWorksheet() : Worksheet;
```


**Returns**

[Worksheet](/nodejs-cpp/worksheet/)

### getCellRow() {#getCellRow--}

Gets the row index of the cell where the function is in.

```javascript
getCellRow() : number;
```


### getCellColumn() {#getCellColumn--}

Gets the column index of the cell where the function is in.

```javascript
getCellColumn() : number;
```


### getCell() {#getCell--}

Gets the Cell object where the function is in.

```javascript
getCell() : Cell;
```


**Returns**

[Cell](/nodejs-cpp/cell/)

**Remarks**

When calculating a formula without setting it to a cell, such as by [Worksheet.CalculateFormula(string, CalculationOptions)](/nodejs-cpp/worksheet.calculateformula(string, calculationoptions)/), the formula will be calculated just like it has been set to cell A1, so both [CellRow](/nodejs-cpp/cellrow/) and [CellRow](/nodejs-cpp/cellrow/) are 0. However, cell A1 in the worksheet may has not been instantiated. So for such kind of situation this property will be null.

### getFunctionName() {#getFunctionName--}

Gets the function name to be calculated.

```javascript
getFunctionName() : string;
```


### getParamCount() {#getParamCount--}

Gets the count of parameters

```javascript
getParamCount() : number;
```


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


