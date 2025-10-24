##TimelineCollection class
## TimelineCollection class
Specifies the collection of all the Timeline objects on the specified worksheet.
Due to MS Excel, Excel 2003 does not support Timeline.
The TimelineCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells.timelines/timelinecollection/capacity) | Gets or sets the number of elements that the array list can contain. |
### Methods
| Method | Description |
| :- | :- |
| [`add(self, pivot, row, column, base_field_name)`](/cells/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.pivottable-int-int-system.string) | Add a new Timeline using PivotTable as data source |
| [`add(self, pivot, dest_cell_name, base_field_name)`](/cells/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.pivottable-system.string-system.string) | Add a new Timeline using PivotTable as data source |
| [`add(self, pivot, row, column, base_field_index)`](/cells/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.pivottable-int-int-int) | Add a new Timeline using PivotTable as data source |
| [`add(self, pivot, dest_cell_name, base_field_index)`](/cells/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.pivottable-system.string-int) | Add a new Timeline using PivotTable as data source |
| [`add(self, pivot, row, column, base_field)`](/cells/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.pivottable-int-int-aspose.cells.pivot.pivotfield) | Add a new Timeline using PivotTable as data source |
| [`add(self, pivot, dest_cell_name, base_field)`](/cells/python-net/aspose.cells.timelines/timelinecollection/add/#aspose.cells.pivot.pivottable-system.string-aspose.cells.pivot.pivotfield) | Add a new Timeline using PivotTable as data source |
| [`copy_to(self, array)`](/cells/python-net/aspose.cells.timelines/timelinecollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [`copy_to(self, index, array, array_index, count)`](/cells/python-net/aspose.cells.timelines/timelinecollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [`index_of(self, item, index)`](/cells/python-net/aspose.cells.timelines/timelinecollection/index_of/#aspose.cells.timelines.timeline-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [`index_of(self, item, index, count)`](/cells/python-net/aspose.cells.timelines/timelinecollection/index_of/#aspose.cells.timelines.timeline-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [`last_index_of(self, item)`](/cells/python-net/aspose.cells.timelines/timelinecollection/last_index_of/#aspose.cells.timelines.timeline) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [`last_index_of(self, item, index)`](/cells/python-net/aspose.cells.timelines/timelinecollection/last_index_of/#aspose.cells.timelines.timeline-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [`last_index_of(self, item, index, count)`](/cells/python-net/aspose.cells.timelines/timelinecollection/last_index_of/#aspose.cells.timelines.timeline-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [`get(self, name)`](/cells/python-net/aspose.cells.timelines/timelinecollection/get/#system.string) | Gets the Timeline  by Timeline's name. |
| [`binary_search(self, item)`](/cells/python-net/aspose.cells.timelines/timelinecollection/binary_search/#aspose.cells.timelines.timeline) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |
### Example
```python
from aspose.cells import CellsFactory, Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType
from datetime import datetime
book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
# Create date style
dateStyle = CellsFactory().create_style()
dateStyle.custom = "m/d/yyyy"
cells.get(0, 1).value = "date"
cells.get(1, 1).value = datetime(2021, 2, 5)
cells.get(2, 1).value = datetime(2022, 3, 8)
cells.get(3, 1).value = datetime(2023, 4, 10)
cells.get(4, 1).value = datetime(2024, 5, 16)
# Set date style
cells.get(1, 1).set_style(dateStyle)
cells.get(2, 1).set_style(dateStyle)
cells.get(3, 1).set_style(dateStyle)
cells.get(4, 1).set_style(dateStyle)
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
pivots = sheet.pivot_tables
# Add a PivotTable
pivotIndex = pivots.add("=Sheet1!A1:C5", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "date")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
# Refresh PivotTable data
pivot.refresh_data()
pivot.calculate_data()
# do your business
book.save("out.xlsx")
```
### See Also
* module [`aspose.cells.timelines`](..)
