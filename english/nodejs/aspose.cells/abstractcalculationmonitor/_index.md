---
title: "AbstractCalculationMonitor"
linktitle: "AbstractCalculationMonitor"
second_title: "Aspose.Cells for Node.js via Java API Reference"
description: "Monitor for user to track the progress of formula calculation."
type: docs
weight: 20
url: /nodejs/aspose.cells/abstractcalculationmonitor/
---

## AbstractCalculationMonitor class

Monitor for user to track the progress of formula calculation.

## Methods

| Name | Description |
| --- | --- |
| [afterCalculate(sheetIndex, rowIndex, colIndex)](#aftercalculate) | Implement this method to do business after one cell has been calculated. |
| [beforeCalculate(sheetIndex, rowIndex, colIndex)](#beforecalculate) | Implement this method to do business before calculating one cell. |
| [getCalculatedValue()](#getcalculatedvalue) | Gets the newly calculated value of the cell. Should be used only in afterCalculate(int, int, int). |
| [getOriginalValue()](#getoriginalvalue) | Gets the old value of the calculated cell. Should be used only in beforeCalculate(int, int, int) and afterCalculate(int, |
| [getValueChanged()](#getvaluechanged) | Whether the cell's value has been changed after the calculation. Should be used only in afterCalculate(int, int, int). |
| [onCircular(circularCellsData)](#oncircular) | Implement this method to do business when calculating formulas with circular references. In the implementation user may  |

### afterCalculate(sheetIndex, rowIndex, colIndex) {#aftercalculate}

Implement this method to do business after one cell has been calculated.

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Number | Index of the sheet that the cell belongs to. |
| rowIndex | Number | Row index of the cell |
| colIndex | Number | Column index of the cell |

### beforeCalculate(sheetIndex, rowIndex, colIndex) {#beforecalculate}

Implement this method to do business before calculating one cell.

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | Number | Index of the sheet that the cell belongs to. |
| rowIndex | Number | Row index of the cell |
| colIndex | Number | Column index of the cell |

### getCalculatedValue() {#getcalculatedvalue}

Gets the newly calculated value of the cell. Should be used only in afterCalculate(int, int, int).

### getOriginalValue() {#getoriginalvalue}

Gets the old value of the calculated cell. Should be used only in beforeCalculate(int, int, int) and afterCalculate(int, int, int).

### getValueChanged() {#getvaluechanged}

Whether the cell's value has been changed after the calculation. Should be used only in afterCalculate(int, int, int).

### onCircular(circularCellsData) {#oncircular}

Implement this method to do business when calculating formulas with circular references. In the implementation user may also set the expected value as calculated result for part/all of those cells so the formula engine will not calculate them recursively.

| Parameter | Type | Description |
| --- | --- | --- |
| circularCellsData | Iterator | IEnumerator with |

**Returns:** boolean — `boolean` Whether the formula engine needs to calculate those cells in circular after this call. True to let the formula engine continue to do calculation for them. False to let the formula engine just mark those cells as Calculated.
