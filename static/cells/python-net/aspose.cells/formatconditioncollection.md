##FormatConditionCollection class
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
| [`add_condition(self, type, operator_type, formula1, formula2)`](/cells/python-net/aspose.cells/formatconditioncollection/add_condition/#aspose.cells.formatconditiontype-aspose.cells.operatortype-system.string-system.string) | Adds a formatting condition. |
| [`add_condition(self, type)`](/cells/python-net/aspose.cells/formatconditioncollection/add_condition/#aspose.cells.formatconditiontype) | Add a format condition. |
| [`remove_area(self, index)`](/cells/python-net/aspose.cells/formatconditioncollection/remove_area/#int) | Removes conditional formatted cell range by index. |
| [`remove_area(self, start_row, start_column, total_rows, total_columns)`](/cells/python-net/aspose.cells/formatconditioncollection/remove_area/#int-int-int-int) | Remove conditional formatting int the range. |
| [`add(self, cell_area, type, operator_type, formula1, formula2)`](/cells/python-net/aspose.cells/formatconditioncollection/add/#aspose.cells.cellarea-aspose.cells.formatconditiontype-aspose.cells.operatortype-system.string-system.string) | Adds a formatting condition and effected cell rang to the FormatConditions
| [`add_area(self, cell_area)`](/cells/python-net/aspose.cells/formatconditioncollection/add_area/#aspose.cells.cellarea) | Adds a conditional formatted cell range. |
| [`get_cell_area(self, index)`](/cells/python-net/aspose.cells/formatconditioncollection/get_cell_area/#int) | Gets the conditional formatted cell range by index. |
| [`remove_condition(self, index)`](/cells/python-net/aspose.cells/formatconditioncollection/remove_condition/#int) | Removes the formatting condition by index. |
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
* module [`aspose.cells`](..)
