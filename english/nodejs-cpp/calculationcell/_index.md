---
title: CalculationCell
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the calculation relevant data about one cell which is being calculated.
type: docs
url: /nodejs-cpp/calculationcell/
---

## CalculationCell class

Represents the calculation relevant data about one cell which is being calculated.

```javascript
class CalculationCell;
```

### Remarks
All objects provided by this class are for "read" purpose only. User should not change any data in the Workbook during the formula calculation process, Otherwise unexpected result or Exception may be caused.

## Methods

| Method | Description |
| --- | --- |
| [getWorkbook()](#getWorkbook--)| Gets the Workbook object. |
| [getWorksheet()](#getWorksheet--)| Gets the Worksheet object where the cell is in. |
| [getCellRow()](#getCellRow--)| Gets the row index of the cell. |
| [getCellColumn()](#getCellColumn--)| Gets the column index of the cell. |
| [getCell()](#getCell--)| Gets the Cell object which is being calculated. |


### getWorkbook() {#getWorkbook--}

Gets the Workbook object.

```javascript
getWorkbook() : Workbook;
```


**Returns**

[Workbook](/nodejs-cpp/workbook/)

### getWorksheet() {#getWorksheet--}

Gets the Worksheet object where the cell is in.

```javascript
getWorksheet() : Worksheet;
```


**Returns**

[Worksheet](/nodejs-cpp/worksheet/)

### getCellRow() {#getCellRow--}

Gets the row index of the cell.

```javascript
getCellRow() : number;
```


### getCellColumn() {#getCellColumn--}

Gets the column index of the cell.

```javascript
getCellColumn() : number;
```


### getCell() {#getCell--}

Gets the Cell object which is being calculated.

```javascript
getCell() : Cell;
```


**Returns**

[Cell](/nodejs-cpp/cell/)


