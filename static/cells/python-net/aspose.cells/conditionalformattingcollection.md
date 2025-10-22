##ConditionalFormattingCollection class
## ConditionalFormattingCollection class
Encapsulates a collection of [`FormatCondition`](/cells/python-net/aspose.cells/formatcondition) objects.
The ConditionalFormattingCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells/conditionalformattingcollection/capacity) | Gets or sets the number of elements that the array list can contain. |
### Methods
| Method | Description |
| :- | :- |
| [`copy_to(self, array)`](/cells/python-net/aspose.cells/conditionalformattingcollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [`copy_to(self, index, array, array_index, count)`](/cells/python-net/aspose.cells/conditionalformattingcollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [`index_of(self, item, index)`](/cells/python-net/aspose.cells/conditionalformattingcollection/index_of/#aspose.cells.formatconditioncollection-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [`index_of(self, item, index, count)`](/cells/python-net/aspose.cells/conditionalformattingcollection/index_of/#aspose.cells.formatconditioncollection-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [`last_index_of(self, item)`](/cells/python-net/aspose.cells/conditionalformattingcollection/last_index_of/#aspose.cells.formatconditioncollection) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [`last_index_of(self, item, index)`](/cells/python-net/aspose.cells/conditionalformattingcollection/last_index_of/#aspose.cells.formatconditioncollection-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [`last_index_of(self, item, index, count)`](/cells/python-net/aspose.cells/conditionalformattingcollection/last_index_of/#aspose.cells.formatconditioncollection-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [`remove_area(self, start_row, start_column, total_rows, total_columns)`](/cells/python-net/aspose.cells/conditionalformattingcollection/remove_area/#int-int-int-int) | Remove all conditional formatting in the range. |
| [`add(self)`](/cells/python-net/aspose.cells/conditionalformattingcollection/add/#) | Adds a FormatConditions to the collection. |
| [`binary_search(self, item)`](/cells/python-net/aspose.cells/conditionalformattingcollection/binary_search/#aspose.cells.formatconditioncollection) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |
### Example
```python
from aspose.cells import CellArea, FormatConditionType, OperatorType, Workbook
from aspose.pydrawing import Color
# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Get Conditional Formatting
cformattings = sheet.conditional_formattings
# Adds an empty conditional formatting
index = cformattings.add()
# Get newly added Conditional formatting
fcs = cformattings[index]
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
# Add condition.
conditionIndex = fcs.add_condition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100")
# Add condition.
conditionIndex2 = fcs.add_condition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100")
# Sets the background color.
fc = fcs[conditionIndex]
fc.style.background_color = Color.red
# Saving the Excel file
workbook.save("output.xls")
```
### See Also
* module [`aspose.cells`](..)
* class [`FormatCondition`](/cells/python-net/aspose.cells/formatcondition)
