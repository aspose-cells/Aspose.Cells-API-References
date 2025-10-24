##SparklineGroupCollection class
## SparklineGroupCollection class
Encapsulates a collection of [`SparklineGroup`](/cells/python-net/aspose.cells.charts/sparklinegroup) objects.
The SparklineGroupCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells.charts/sparklinegroupcollection/capacity) | Gets or sets the number of elements that the array list can contain. |
### Methods
| Method | Description |
| :- | :- |
| [`add(self, type)`](/cells/python-net/aspose.cells.charts/sparklinegroupcollection/add/#aspose.cells.charts.sparklinetype) | Adds an [`SparklineGroup`](/cells/python-net/aspose.cells.charts/sparklinegroup) with a [`Sparkline`](/cells/python-net/aspose.cells.charts/sparkline) to the collection. |
| [`add(self, type, data_range, is_vertical, location_range)`](/cells/python-net/aspose.cells.charts/sparklinegroupcollection/add/#aspose.cells.charts.sparklinetype-system.string-bool-aspose.cells.cellarea) | Adds an [`SparklineGroup`](/cells/python-net/aspose.cells.charts/sparklinegroup) with [`Sparkline`](/cells/python-net/aspose.cells.charts/sparkline) to the collection. |
| [`copy_to(self, array)`](/cells/python-net/aspose.cells.charts/sparklinegroupcollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [`copy_to(self, index, array, array_index, count)`](/cells/python-net/aspose.cells.charts/sparklinegroupcollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [`index_of(self, item, index)`](/cells/python-net/aspose.cells.charts/sparklinegroupcollection/index_of/#aspose.cells.charts.sparklinegroup-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [`index_of(self, item, index, count)`](/cells/python-net/aspose.cells.charts/sparklinegroupcollection/index_of/#aspose.cells.charts.sparklinegroup-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [`last_index_of(self, item)`](/cells/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#aspose.cells.charts.sparklinegroup) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [`last_index_of(self, item, index)`](/cells/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#aspose.cells.charts.sparklinegroup-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [`last_index_of(self, item, index, count)`](/cells/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#aspose.cells.charts.sparklinegroup-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [`clear_sparklines(self, cell_area)`](/cells/python-net/aspose.cells.charts/sparklinegroupcollection/clear_sparklines/#aspose.cells.cellarea) | Clears the sparklines that is inside an area of cells. |
| [`clear_sparkline_groups(self, cell_area)`](/cells/python-net/aspose.cells.charts/sparklinegroupcollection/clear_sparkline_groups/#aspose.cells.cellarea) | Clears the sparkline groups that overlaps an area of cells. |
| [`binary_search(self, item)`](/cells/python-net/aspose.cells.charts/sparklinegroupcollection/binary_search/#aspose.cells.charts.sparklinegroup) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |
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
idx = sheet.sparkline_groups.add(SparklineType.LINE, "A1:D1", False, ca)
group = sheet.sparkline_groups[idx]
group.sparklines.add(sheet.name + "!A1:D1", 0, 4)
book.save("output.xlsx", SaveFormat.XLSX)
```
### See Also
* module [`aspose.cells.charts`](..)
* class [`Sparkline`](/cells/python-net/aspose.cells.charts/sparkline)
* class [`SparklineGroup`](/cells/python-net/aspose.cells.charts/sparklinegroup)
