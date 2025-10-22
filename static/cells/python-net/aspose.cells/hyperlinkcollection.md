##HyperlinkCollection class
## HyperlinkCollection class
Encapsulates a collection of [`Hyperlink`](/cells/python-net/aspose.cells/hyperlink) objects.
The HyperlinkCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells/hyperlinkcollection/capacity) | Gets or sets the number of elements that the array list can contain. |
### Methods
| Method | Description |
| :- | :- |
| [`add(self, first_row, first_column, total_rows, total_columns, address)`](/cells/python-net/aspose.cells/hyperlinkcollection/add/#int-int-int-int-system.string) | Adds a hyperlink to a specified cell or a range of cells. |
| [`add(self, cell_name, total_rows, total_columns, address)`](/cells/python-net/aspose.cells/hyperlinkcollection/add/#system.string-int-int-system.string) | Adds a hyperlink to a specified cell or a range of cells. |
| [`add(self, start_cell_name, end_cell_name, address, text_to_display, screen_tip)`](/cells/python-net/aspose.cells/hyperlinkcollection/add/#system.string-system.string-system.string-system.string-system.string) | Adds a hyperlink to a specified cell or a range of cells. |
| [`copy_to(self, array)`](/cells/python-net/aspose.cells/hyperlinkcollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [`copy_to(self, index, array, array_index, count)`](/cells/python-net/aspose.cells/hyperlinkcollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [`index_of(self, item, index)`](/cells/python-net/aspose.cells/hyperlinkcollection/index_of/#aspose.cells.hyperlink-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [`index_of(self, item, index, count)`](/cells/python-net/aspose.cells/hyperlinkcollection/index_of/#aspose.cells.hyperlink-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [`last_index_of(self, item)`](/cells/python-net/aspose.cells/hyperlinkcollection/last_index_of/#aspose.cells.hyperlink) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [`last_index_of(self, item, index)`](/cells/python-net/aspose.cells/hyperlinkcollection/last_index_of/#aspose.cells.hyperlink-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [`last_index_of(self, item, index, count)`](/cells/python-net/aspose.cells/hyperlinkcollection/last_index_of/#aspose.cells.hyperlink-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [`binary_search(self, item)`](/cells/python-net/aspose.cells/hyperlinkcollection/binary_search/#aspose.cells.hyperlink) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |
### Example
```python
from aspose.cells import Workbook
# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Get Hyperlinks Collection
hyperlinks = worksheet.hyperlinks
# Adding a hyperlink to a URL at "A1" cell
hyperlinks.add("A1", 1, 1, "http://www.aspose.com")
# Saving the Excel file
workbook.save("book1.xls")
```
### See Also
* module [`aspose.cells`](..)
* class [`Hyperlink`](/cells/python-net/aspose.cells/hyperlink)
