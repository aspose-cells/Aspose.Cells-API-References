---
title: AbstractCalculationMonitor
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 30
url: /python-net/aspose.cells/abstractcalculationmonitor/
---

## AbstractCalculationMonitor class

Monitor for user to track the progress of formula calculation.

The AbstractCalculationMonitor type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|original_value|Gets the old value of the calculated cell.<br/>            Should be used only in|
|value_changed|Whether the cell's value has been changed after the calculation.<br/>            Should be used only in|
|calculated_value|Gets the newly calculated value of the cell.<br/>            Should be used only in|
## Methods
| Name | Description |
| :- | :- |
|before_calculate(sheet_index, row_index, col_index)|Implement this method to do business before calculating one cell.|
|after_calculate(sheet_index, row_index, col_index)|Implement this method to do business after one cell has been calculated.|
|on_circular(circular_cells_data)|Implement this method to do business when calculating formulas with circular references.|

### See Also

* namespace [aspose.cells](/python-net/aspose.cells/)
* assembly [Aspose.Cells](/python-net/)

