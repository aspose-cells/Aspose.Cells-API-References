---
title: AbstractFormulaChangeMonitor
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Monitor for the user to track the change of formulas during certain operations.
type: docs
url: /javascript-cpp/abstractformulachangemonitor/
---

## AbstractFormulaChangeMonitor class

Monitor for the user to track the change of formulas during certain operations.

```javascript
abstract class AbstractFormulaChangeMonitor;
```

### Remarks
For example, while deleting/inserting range of cells, formulas of other cells may be changed because of the shift of references. Please note, methods in the monitor may be invoked multiple times for one object which contains the formula.

## Methods

| Method | Description |
| --- | --- |
| abstract [onCellFormulaChanged(number, number, number)](#onCellFormulaChanged-number-number-number-)| The event that will be triggered when the formula in a cell is changed. |
| abstract [onFormatConditionFormulaChanged(FormatCondition)](#onFormatConditionFormulaChanged-formatcondition-)| The event that will be triggered when the formula of FormatCondition is changed. |


### onCellFormulaChanged(number, number, number) {#onCellFormulaChanged-number-number-number-}

The event that will be triggered when the formula in a cell is changed.

```javascript
abstract onCellFormulaChanged(sheetIndex: number, rowIndex: number, columnIndex: number) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| sheetIndex | number | The sheet index of the changed cell |
| rowIndex | number | The row index of the changed cell |
| columnIndex | number | The column index of the changed cell |

### onFormatConditionFormulaChanged(FormatCondition) {#onFormatConditionFormulaChanged-formatcondition-}

The event that will be triggered when the formula of FormatCondition is changed.

```javascript
abstract onFormatConditionFormulaChanged(fc: FormatCondition) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| fc | [FormatCondition](../formatcondition/) | The FormatCondition object whose formula is changed |


