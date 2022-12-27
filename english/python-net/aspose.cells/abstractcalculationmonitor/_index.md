---
title: AbstractCalculationMonitor class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 30
url: /python-net/aspose.cells/abstractcalculationmonitor/
is_root: false
---

## AbstractCalculationMonitor class

Monitor for user to track the progress of formula calculation.



The AbstractCalculationMonitor type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [original_value](/cells/python-net/aspose.cells/abstractcalculationmonitor/original_value) | Gets the old value of the calculated cell.<br/>Should be used only in [AbstractCalculationMonitor.before_calculate(sheet_index, row_index, col_index)](/cells/python-net/aspose.cells/abstractcalculationmonitor/before_calculate) and [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/python-net/aspose.cells/abstractcalculationmonitor/after_calculate). |
| [value_changed](/cells/python-net/aspose.cells/abstractcalculationmonitor/value_changed) | Whether the cell's value has been changed after the calculation.<br/>Should be used only in [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/python-net/aspose.cells/abstractcalculationmonitor/after_calculate). |
| [calculated_value](/cells/python-net/aspose.cells/abstractcalculationmonitor/calculated_value) | Gets the newly calculated value of the cell.<br/>Should be used only in [AbstractCalculationMonitor.after_calculate(sheet_index, row_index, col_index)](/cells/python-net/aspose.cells/abstractcalculationmonitor/after_calculate). |


### Methods
| Method | Description |
| :- | :- |
| [before_calculate(sheet_index, row_index, col_index)](/cells/python-net/aspose.cells/abstractcalculationmonitor/before_calculate/#int-int-int) | Implement this method to do business before calculating one cell. |
| [after_calculate(sheet_index, row_index, col_index)](/cells/python-net/aspose.cells/abstractcalculationmonitor/after_calculate/#int-int-int) | Implement this method to do business after one cell has been calculated. |
| [on_circular(circular_cells_data)](/cells/python-net/aspose.cells/abstractcalculationmonitor/on_circular/#collections.abc.Iterator) | Implement this method to do business when calculating formulas with circular references. |


### See Also

* module [aspose.cells](../)
