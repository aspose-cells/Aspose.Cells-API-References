##TextBoxCollection class
## TextBoxCollection class
Encapsulates a collection of [`TextBox`](/cells/python-net/aspose.cells.drawing/textbox) objects.
The TextBoxCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells.drawing/textboxcollection/capacity) | Gets or sets the number of elements that the array list can contain. |
### Methods
| Method | Description |
| :- | :- |
| [`copy_to(self, array)`](/cells/python-net/aspose.cells.drawing/textboxcollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [`copy_to(self, index, array, array_index, count)`](/cells/python-net/aspose.cells.drawing/textboxcollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [`index_of(self, item, index)`](/cells/python-net/aspose.cells.drawing/textboxcollection/index_of/#aspose.cells.drawing.textbox-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [`index_of(self, item, index, count)`](/cells/python-net/aspose.cells.drawing/textboxcollection/index_of/#aspose.cells.drawing.textbox-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [`last_index_of(self, item)`](/cells/python-net/aspose.cells.drawing/textboxcollection/last_index_of/#aspose.cells.drawing.textbox) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [`last_index_of(self, item, index)`](/cells/python-net/aspose.cells.drawing/textboxcollection/last_index_of/#aspose.cells.drawing.textbox-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [`last_index_of(self, item, index, count)`](/cells/python-net/aspose.cells.drawing/textboxcollection/last_index_of/#aspose.cells.drawing.textbox-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [`get(self, name)`](/cells/python-net/aspose.cells.drawing/textboxcollection/get/#system.string) | Gets the [`TextBox`](/cells/python-net/aspose.cells.drawing/textbox) element by the name. |
| [`add(self, upper_left_row, upper_left_column, height, width)`](/cells/python-net/aspose.cells.drawing/textboxcollection/add/#int-int-int-int) | Adds a textbox to the collection. |
| [`binary_search(self, item)`](/cells/python-net/aspose.cells.drawing/textboxcollection/binary_search/#aspose.cells.drawing.textbox) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |
### Example
```python
from aspose.cells import Workbook
# Instantiating a Workbook object
workbook = Workbook()
# get collection object
textBoxCollection = workbook.worksheets[0].text_boxes
# add a textbox
textBoxCollection.add(1, 1, 50, 100)
for tbox in textBoxCollection:
pass
```
### See Also
* module [`aspose.cells.drawing`](..)
* class [`TextBox`](/cells/python-net/aspose.cells.drawing/textbox)
