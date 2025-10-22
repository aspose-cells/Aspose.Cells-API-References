##SlicerCollection class
## SlicerCollection class
Specifies the collection of all the Slicer objects on the specified worksheet.
The SlicerCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells.slicers/slicercollection/capacity) | Gets or sets the number of elements that the array list can contain. |
### Methods
| Method | Description |
| :- | :- |
| [`add(self, pivot, dest_cell_name, base_field_name)`](/cells/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.pivottable-system.string-system.string) | Add a new Slicer using PivotTable as data source |
| [`add(self, pivot, row, column, base_field_name)`](/cells/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.pivottable-int-int-system.string) | Add a new Slicer using PivotTable as data source |
| [`add(self, pivot, row, column, base_field_index)`](/cells/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.pivottable-int-int-int) | Add a new Slicer using PivotTable as data source |
| [`add(self, pivot, dest_cell_name, base_field_index)`](/cells/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.pivottable-system.string-int) | Add a new Slicer using PivotTable as data source |
| [`add(self, pivot, row, column, base_field)`](/cells/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.pivottable-int-int-aspose.cells.pivot.pivotfield) | Add a new Slicer using PivotTable as data source |
| [`add(self, pivot, dest_cell_name, base_field)`](/cells/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.pivot.pivottable-system.string-aspose.cells.pivot.pivotfield) | Add a new Slicer using PivotTable as data source |
| [`add(self, table, index, dest_cell_name)`](/cells/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.tables.listobject-int-system.string) | Add a new Slicer using ListObjet as data source |
| [`add(self, table, list_column, dest_cell_name)`](/cells/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.tables.listobject-aspose.cells.tables.listcolumn-system.string) | Add a new Slicer using ListObjet as data source |
| [`add(self, table, list_column, row, column)`](/cells/python-net/aspose.cells.slicers/slicercollection/add/#aspose.cells.tables.listobject-aspose.cells.tables.listcolumn-int-int) | Add a new Slicer using ListObjet as data source |
| [`copy_to(self, array)`](/cells/python-net/aspose.cells.slicers/slicercollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [`copy_to(self, index, array, array_index, count)`](/cells/python-net/aspose.cells.slicers/slicercollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [`index_of(self, item, index)`](/cells/python-net/aspose.cells.slicers/slicercollection/index_of/#aspose.cells.slicers.slicer-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [`index_of(self, item, index, count)`](/cells/python-net/aspose.cells.slicers/slicercollection/index_of/#aspose.cells.slicers.slicer-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [`last_index_of(self, item)`](/cells/python-net/aspose.cells.slicers/slicercollection/last_index_of/#aspose.cells.slicers.slicer) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [`last_index_of(self, item, index)`](/cells/python-net/aspose.cells.slicers/slicercollection/last_index_of/#aspose.cells.slicers.slicer-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [`last_index_of(self, item, index, count)`](/cells/python-net/aspose.cells.slicers/slicercollection/last_index_of/#aspose.cells.slicers.slicer-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [`get(self, name)`](/cells/python-net/aspose.cells.slicers/slicercollection/get/#system.string) | Gets the Slicer  by slicer's name. |
| [`binary_search(self, item)`](/cells/python-net/aspose.cells.slicers/slicercollection/binary_search/#aspose.cells.slicers.slicer) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |
### Example
```python
from aspose.cells import Workbook
from aspose.cells.pivot import PivotFieldType, PivotTableStyleType
book = Workbook()
sheet = book.worksheets[0]
cells = sheet.cells
cells.get(0, 0).value = "fruit"
cells.get(1, 0).value = "grape"
cells.get(2, 0).value = "blueberry"
cells.get(3, 0).value = "kiwi"
cells.get(4, 0).value = "cherry"
cells.get(5, 0).value = "grape"
cells.get(6, 0).value = "blueberry"
cells.get(7, 0).value = "kiwi"
cells.get(8, 0).value = "cherry"
cells.get(0, 1).value = "year"
cells.get(1, 1).value = 2020
cells.get(2, 1).value = 2020
cells.get(3, 1).value = 2020
cells.get(4, 1).value = 2020
cells.get(5, 1).value = 2021
cells.get(6, 1).value = 2021
cells.get(7, 1).value = 2021
cells.get(8, 1).value = 2021
cells.get(0, 2).value = "amount"
cells.get(1, 2).value = 50
cells.get(2, 2).value = 60
cells.get(3, 2).value = 70
cells.get(4, 2).value = 80
cells.get(5, 2).value = 90
cells.get(6, 2).value = 100
cells.get(7, 2).value = 110
cells.get(8, 2).value = 120
pivots = sheet.pivot_tables
pivotIndex = pivots.add("=Sheet1!A1:C9", "A12", "TestPivotTable")
pivot = pivots[pivotIndex]
pivot.add_field_to_area(PivotFieldType.ROW, "fruit")
pivot.add_field_to_area(PivotFieldType.COLUMN, "year")
pivot.add_field_to_area(PivotFieldType.DATA, "amount")
pivot.pivot_table_style_type = PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM10
pivot.refresh_data()
pivot.calculate_data()
slicers = sheet.slicers
tableIndex = sheet.list_objects.add("A1", "C9", True)
table = sheet.list_objects[tableIndex]
# do your business
book.save("out.xlsx")
```
### See Also
* module [`aspose.cells.slicers`](..)
