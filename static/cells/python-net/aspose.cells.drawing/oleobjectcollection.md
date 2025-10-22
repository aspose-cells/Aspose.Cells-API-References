##OleObjectCollection class
## OleObjectCollection class
Represents embedded OLE objects.
The OleObjectCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells.drawing/oleobjectcollection/capacity) | Gets or sets the number of elements that the array list can contain. |
### Methods
| Method | Description |
| :- | :- |
| [`add(self, upper_left_row, upper_left_column, height, width, image_data)`](/cells/python-net/aspose.cells.drawing/oleobjectcollection/add/#int-int-int-int-bytes) | Adds an OleObject to the collection. |
| [`add(self, upper_left_row, upper_left_column, height, width, image_data, linked_file)`](/cells/python-net/aspose.cells.drawing/oleobjectcollection/add/#int-int-int-int-bytes-system.string) | Adds a linked OleObject to the collection. |
| [`copy_to(self, array)`](/cells/python-net/aspose.cells.drawing/oleobjectcollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [`copy_to(self, index, array, array_index, count)`](/cells/python-net/aspose.cells.drawing/oleobjectcollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [`index_of(self, item, index)`](/cells/python-net/aspose.cells.drawing/oleobjectcollection/index_of/#aspose.cells.drawing.oleobject-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [`index_of(self, item, index, count)`](/cells/python-net/aspose.cells.drawing/oleobjectcollection/index_of/#aspose.cells.drawing.oleobject-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [`last_index_of(self, item)`](/cells/python-net/aspose.cells.drawing/oleobjectcollection/last_index_of/#aspose.cells.drawing.oleobject) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [`last_index_of(self, item, index)`](/cells/python-net/aspose.cells.drawing/oleobjectcollection/last_index_of/#aspose.cells.drawing.oleobject-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [`last_index_of(self, item, index, count)`](/cells/python-net/aspose.cells.drawing/oleobjectcollection/last_index_of/#aspose.cells.drawing.oleobject-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [`binary_search(self, item)`](/cells/python-net/aspose.cells.drawing/oleobjectcollection/binary_search/#aspose.cells.drawing.oleobject) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |
### See Also
* module [`aspose.cells.drawing`](..)
