---
title: "AbstractCalculationMonitor Class"
linktitle: "AbstractCalculationMonitor"
articleTitle: "AbstractCalculationMonitor"
second_title: "Aspose.Cells for Python via Java"
description: "Monitor for user to track the progress of formula calculation."
type: docs
weight: 20
url: /python-java/asposecells.api/abstractcalculationmonitor/
---

## AbstractCalculationMonitor class

Monitor for user to track the progress of formula calculation.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [OriginalValue](#originalvalue) | Object | Gets the old value of the calculated cell. Should be used only in beforeCalculate(int, int, int) and afterCalculate(int, |
| [ValueChanged](#valuechanged) | boolean | Whether the cell's value has been changed after the calculation. Should be used only in afterCalculate(int, int, int) . |
| [CalculatedValue](#calculatedvalue) | Object | Gets the newly calculated value of the cell. Should be used only in afterCalculate(int, int, int) . |

## Methods

| Name | Description |
| --- | --- |
| [beforeCalculate](#beforecalculate) | Implement this method to do business before calculating one cell. |
| [afterCalculate](#aftercalculate) | Implement this method to do business after one cell has been calculated. |
| [onCircular](#oncircular) | Implement this method to do business when calculating formulas with circular references.

In the implementation user may |

### AbstractCalculationMonitor.OriginalValue property {#originalvalue}

Gets the old value of the calculated cell. Should be used only in beforeCalculate(int, int, int) and afterCalculate(int, int, int) .

**Type:** Object

### AbstractCalculationMonitor.ValueChanged property {#valuechanged}

Whether the cell's value has been changed after the calculation. Should be used only in afterCalculate(int, int, int) .

**Type:** boolean

### AbstractCalculationMonitor.CalculatedValue property {#calculatedvalue}

Gets the newly calculated value of the cell. Should be used only in afterCalculate(int, int, int) .

**Type:** Object

### beforeCalculate(sheetIndex, rowIndex, colIndex) {#beforecalculate}

Implement this method to do business before calculating one cell.

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | int | Index of the sheet that the cell belongs to. |
| rowIndex | int | Row index of the cell |
| colIndex | int | Column index of the cell |

### afterCalculate(sheetIndex, rowIndex, colIndex) {#aftercalculate}

Implement this method to do business after one cell has been calculated.

| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | int | Index of the sheet that the cell belongs to. |
| rowIndex | int | Row index of the cell |
| colIndex | int | Column index of the cell |

### onCircular(circularCellsData) {#oncircular}

Implement this method to do business when calculating formulas with circular references.

In the implementation user may also set the expected value as calculated result for part/all of those cells so the formula engine will not calculate them recursively.

| Parameter | Type | Description |
| --- | --- | --- |
| circularCellsData | Iterator | IEnumerator with CalculationCell items representing cells that depend on circular references. |

**Returns:** Whether the formula engine needs to calculate those cells in circular after this call. True to let the formula engine continue to do calculation for them. False to let the formula engine just mark those cells as Calculated.
