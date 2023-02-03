---
title: FormatConditionCollection class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 700
url: /python-net/aspose.cells/formatconditioncollection/
is_root: false
---

## FormatConditionCollection class

Represents conditional formatting.
The FormatConditions can contain up to three conditional formats.



The FormatConditionCollection type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [count](/cells/python-net/aspose.cells/formatconditioncollection/count) | Gets the count of the conditions. |
| [range_count](/cells/python-net/aspose.cells/formatconditioncollection/range_count) | Gets count of conditionally formatted ranges. |



Gets the formatting condition by index.
### Indexer
| Name | Description |
| :- | :- |
| [index] | the index of the formatting condition to return. |


### Methods
| Method | Description |
| :- | :- |
| [add_condition(type, operator_type, formula1, formula2)](/cells/python-net/aspose.cells/formatconditioncollection/add_condition/#FormatConditionType-OperatorType-str-str) | Adds a formatting condition. |
| [add_condition(type)](/cells/python-net/aspose.cells/formatconditioncollection/add_condition/#FormatConditionType) | Add a format condition. |
| [remove_area(index)](/cells/python-net/aspose.cells/formatconditioncollection/remove_area/#int) | Removes conditional formatted cell range by index. |
| [remove_area(start_row, start_column, total_rows, total_columns)](/cells/python-net/aspose.cells/formatconditioncollection/remove_area/#int-int-int-int) | Remove conditional formatting int the range. |
| [add(cell_area, type, operator_type, formula1, formula2)](/cells/python-net/aspose.cells/formatconditioncollection/add/#CellArea-FormatConditionType-OperatorType-str-str) | Adds a formatting condition and effected cell rang to the FormatConditions<br/>The FormatConditions can contain up to three conditional formats.<br/>References to the other sheets are not allowed in the formulas of conditional formatting. |
| [add_area(cell_area)](/cells/python-net/aspose.cells/formatconditioncollection/add_area/#CellArea) | Adds a conditional formatted cell range. |
| [get_cell_area(index)](/cells/python-net/aspose.cells/formatconditioncollection/get_cell_area/#int) | Gets the conditional formatted cell range by index. |
| [remove_condition(index)](/cells/python-net/aspose.cells/formatconditioncollection/remove_condition/#int) | Removes the formatting condition by index. |



### Example 


```python
from aspose.cells import CellArea, FormatConditionType, OperatorType, Workbook
from aspose.pydrawing import Color

# Create a new Workbook.
workbook = Workbook()
# Get the first worksheet.
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea()
ca.start_row = 0
ca.end_row = 0
ca.start_column = 0
ca.end_column = 0
fcs.add_area(ca)
ca = CellArea()
ca.start_row = 1
ca.end_row = 1
ca.start_column = 1
ca.end_column = 1
fcs.add_area(ca)
# Adds condition.
conditionIndex = fcs.add_condition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100")
# Adds condition.
conditionIndex2 = fcs.add_condition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100")
# Sets the background color.
fc = fcs[conditionIndex]
fc.style.background_color = Color.red
# Saving the Excel file
workbook.save("output.xls")

```
### See Also

* module [aspose.cells](../)
