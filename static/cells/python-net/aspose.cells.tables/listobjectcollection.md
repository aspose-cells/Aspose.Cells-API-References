##ListObjectCollection class
## ListObjectCollection class
Represents a collection of [`ListObject`](/cells/python-net/aspose.cells.tables/listobject) objects in the worksheet.
The ListObjectCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells.tables/listobjectcollection/capacity) | Gets or sets the number of elements that the array list can contain. |
### Methods
| Method | Description |
| :- | :- |
| [`get(self, index)`](/cells/python-net/aspose.cells.tables/listobjectcollection/get/#int) | Add API for Python Via .Net.since this[int] is unsupported |
| [`get(self, table_name)`](/cells/python-net/aspose.cells.tables/listobjectcollection/get/#system.string) | Add API for Python Via .Net.since this[string] is unsupported |
| [`add(self, start_row, start_column, end_row, end_column, has_headers)`](/cells/python-net/aspose.cells.tables/listobjectcollection/add/#int-int-int-int-bool) | Adds a ListObject to the worksheet. |
| [`add(self, start_cell, end_cell, has_headers)`](/cells/python-net/aspose.cells.tables/listobjectcollection/add/#system.string-system.string-bool) | Adds a ListObject to the worksheet. |
| [`copy_to(self, array)`](/cells/python-net/aspose.cells.tables/listobjectcollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [`copy_to(self, index, array, array_index, count)`](/cells/python-net/aspose.cells.tables/listobjectcollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [`index_of(self, item, index)`](/cells/python-net/aspose.cells.tables/listobjectcollection/index_of/#aspose.cells.tables.listobject-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [`index_of(self, item, index, count)`](/cells/python-net/aspose.cells.tables/listobjectcollection/index_of/#aspose.cells.tables.listobject-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [`last_index_of(self, item)`](/cells/python-net/aspose.cells.tables/listobjectcollection/last_index_of/#aspose.cells.tables.listobject) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [`last_index_of(self, item, index)`](/cells/python-net/aspose.cells.tables/listobjectcollection/last_index_of/#aspose.cells.tables.listobject-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [`last_index_of(self, item, index, count)`](/cells/python-net/aspose.cells.tables/listobjectcollection/last_index_of/#aspose.cells.tables.listobject-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [`update_column_name(self)`](/cells/python-net/aspose.cells.tables/listobjectcollection/update_column_name/#) | Update all column name of the tables. |
| [`binary_search(self, item)`](/cells/python-net/aspose.cells.tables/listobjectcollection/binary_search/#aspose.cells.tables.listobject) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |
### See Also
* module [`aspose.cells.tables`](..)
* class [`ListObject`](/cells/python-net/aspose.cells.tables/listobject)
