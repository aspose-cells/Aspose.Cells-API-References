##SparklineCollection class
## SparklineCollection class
Encapsulates a collection of [`Sparkline`](/cells/python-net/aspose.cells.charts/sparkline) objects.
The SparklineCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells.charts/sparklinecollection/capacity) | Gets or sets the number of elements that the array list can contain. |
### Methods
| Method | Description |
| :- | :- |
| [`copy_to(self, array)`](/cells/python-net/aspose.cells.charts/sparklinecollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [`copy_to(self, index, array, array_index, count)`](/cells/python-net/aspose.cells.charts/sparklinecollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [`index_of(self, item, index)`](/cells/python-net/aspose.cells.charts/sparklinecollection/index_of/#aspose.cells.charts.sparkline-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [`index_of(self, item, index, count)`](/cells/python-net/aspose.cells.charts/sparklinecollection/index_of/#aspose.cells.charts.sparkline-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [`last_index_of(self, item)`](/cells/python-net/aspose.cells.charts/sparklinecollection/last_index_of/#aspose.cells.charts.sparkline) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [`last_index_of(self, item, index)`](/cells/python-net/aspose.cells.charts/sparklinecollection/last_index_of/#aspose.cells.charts.sparkline-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [`last_index_of(self, item, index, count)`](/cells/python-net/aspose.cells.charts/sparklinecollection/last_index_of/#aspose.cells.charts.sparkline-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [`add(self, data_range, row, column)`](/cells/python-net/aspose.cells.charts/sparklinecollection/add/#system.string-int-int) | Add a sparkline. |
| [`binary_search(self, item)`](/cells/python-net/aspose.cells.charts/sparklinecollection/binary_search/#aspose.cells.charts.sparkline) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |
### Example
```python
from aspose.cells import CellArea, SaveFormat, Workbook
from aspose.cells.charts import SparklineType
book = Workbook()
sheet = book.worksheets[0]
sheet.cells.get("A1").put_value(5)
sheet.cells.get("B1").put_value(2)
sheet.cells.get("C1").put_value(1)
sheet.cells.get("D1").put_value(3)
#  Define the CellArea
ca = CellArea()
ca.start_column = 4
ca.end_column = 4
ca.start_row = 0
ca.end_row = 0
idx = sheet.sparkline_groups.add(SparklineType.LINE, sheet.name + "!A1:D1", False, ca)
group = sheet.sparkline_groups[idx]
group.sparklines.add(sheet.name + "!A1:D1", 0, 4)
book.save("output.xlsx", SaveFormat.XLSX)
```
### See Also
* module [`aspose.cells.charts`](..)
* class [`Sparkline`](/cells/python-net/aspose.cells.charts/sparkline)
