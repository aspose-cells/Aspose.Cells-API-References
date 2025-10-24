##CellWatchCollection class
## CellWatchCollection class
Represents the collection of cells on this worksheet being watched in the 'watch window'.
The CellWatchCollection type exposes the following members:
### Constructors
| Constructor | Description |
| :- | :- |
| [`__init__(self)`](/cells/python-net/aspose.cells/cellwatchcollection/__init__/#) | Constructs a new instance of CellWatchCollection |
### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells/cellwatchcollection/capacity) | Gets or sets the number of elements that the array list can contain. |
### Methods
| Method | Description |
| :- | :- |
| [`add(self, row, column)`](/cells/python-net/aspose.cells/cellwatchcollection/add/#int-int) | Adds [`CellWatch`](/cells/python-net/aspose.cells/cellwatch) with row and column. |
| [`add(self, cell_name)`](/cells/python-net/aspose.cells/cellwatchcollection/add/#system.string) | Adds [`CellWatch`](/cells/python-net/aspose.cells/cellwatch) with the name the of cell. |
| [`copy_to(self, array)`](/cells/python-net/aspose.cells/cellwatchcollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [`copy_to(self, index, array, array_index, count)`](/cells/python-net/aspose.cells/cellwatchcollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [`index_of(self, item, index)`](/cells/python-net/aspose.cells/cellwatchcollection/index_of/#aspose.cells.cellwatch-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [`index_of(self, item, index, count)`](/cells/python-net/aspose.cells/cellwatchcollection/index_of/#aspose.cells.cellwatch-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [`last_index_of(self, item)`](/cells/python-net/aspose.cells/cellwatchcollection/last_index_of/#aspose.cells.cellwatch) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [`last_index_of(self, item, index)`](/cells/python-net/aspose.cells/cellwatchcollection/last_index_of/#aspose.cells.cellwatch-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [`last_index_of(self, item, index, count)`](/cells/python-net/aspose.cells/cellwatchcollection/last_index_of/#aspose.cells.cellwatch-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [`get(self, cell_name)`](/cells/python-net/aspose.cells/cellwatchcollection/get/#system.string) | Gets and sets [`CellWatch`](/cells/python-net/aspose.cells/cellwatch) by the name of the cell. |
| [`binary_search(self, item)`](/cells/python-net/aspose.cells/cellwatchcollection/binary_search/#aspose.cells.cellwatch) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |
### Example
```python
from aspose.cells import Workbook
# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet.
sheet = workbook.worksheets[0]
#  Add Cell Watch Item into the watch window
sheet.cell_watches.add("B2")
```
### See Also
* module [`aspose.cells`](..)
* class [`CellWatch`](/cells/python-net/aspose.cells/cellwatch)
