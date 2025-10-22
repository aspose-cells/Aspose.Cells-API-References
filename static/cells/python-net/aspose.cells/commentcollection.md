##CommentCollection class
## CommentCollection class
Encapsulates a collection of [`Comment`](/cells/python-net/aspose.cells/comment) objects.
The CommentCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells/commentcollection/capacity) | Gets or sets the number of elements that the array list can contain. |
### Methods
| Method | Description |
| :- | :- |
| [`add_threaded_comment(self, row, column, text, author)`](/cells/python-net/aspose.cells/commentcollection/add_threaded_comment/#int-int-system.string-aspose.cells.threadedcommentauthor) | Adds a threaded comment. |
| [`add_threaded_comment(self, cell_name, text, author)`](/cells/python-net/aspose.cells/commentcollection/add_threaded_comment/#system.string-system.string-aspose.cells.threadedcommentauthor) | Adds a threaded comment. |
| [`get_threaded_comments(self, row, column)`](/cells/python-net/aspose.cells/commentcollection/get_threaded_comments/#int-int) | Gets the threaded comments by row and column index. |
| [`get_threaded_comments(self, cell_name)`](/cells/python-net/aspose.cells/commentcollection/get_threaded_comments/#system.string) | Gets the threaded comments by cell name. |
| [`add(self, row, column)`](/cells/python-net/aspose.cells/commentcollection/add/#int-int) | Adds a comment to the collection. |
| [`add(self, cell_name)`](/cells/python-net/aspose.cells/commentcollection/add/#system.string) | Adds a comment to the collection. |
| [`get(self, row, column)`](/cells/python-net/aspose.cells/commentcollection/get/#int-int) | Add API for Python Via .Net.since this[int, int] is unsupported |
| [`get(self, index)`](/cells/python-net/aspose.cells/commentcollection/get/#int) | Gets the [`Comment`](/cells/python-net/aspose.cells/comment) element at the specified index. |
| [`get(self, cell_name)`](/cells/python-net/aspose.cells/commentcollection/get/#system.string) | Gets the [`Comment`](/cells/python-net/aspose.cells/comment) element at the specified cell. |
| [`remove_at(self, cell_name)`](/cells/python-net/aspose.cells/commentcollection/remove_at/#system.string) | Removes the comment of the specific cell. |
| [`remove_at(self, row, column)`](/cells/python-net/aspose.cells/commentcollection/remove_at/#int-int) | Removes the comment of the specific cell. |
| [`copy_to(self, array)`](/cells/python-net/aspose.cells/commentcollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [`copy_to(self, index, array, array_index, count)`](/cells/python-net/aspose.cells/commentcollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [`index_of(self, item, index)`](/cells/python-net/aspose.cells/commentcollection/index_of/#aspose.cells.comment-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [`index_of(self, item, index, count)`](/cells/python-net/aspose.cells/commentcollection/index_of/#aspose.cells.comment-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [`last_index_of(self, item)`](/cells/python-net/aspose.cells/commentcollection/last_index_of/#aspose.cells.comment) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [`last_index_of(self, item, index)`](/cells/python-net/aspose.cells/commentcollection/last_index_of/#aspose.cells.comment-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [`last_index_of(self, item, index, count)`](/cells/python-net/aspose.cells/commentcollection/last_index_of/#aspose.cells.comment-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [`binary_search(self, item)`](/cells/python-net/aspose.cells/commentcollection/binary_search/#aspose.cells.comment) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |
### Example
```python
from aspose.cells import Workbook
workbook = Workbook()
comments = workbook.worksheets[0].comments
```
### See Also
* module [`aspose.cells`](..)
* class [`Comment`](/cells/python-net/aspose.cells/comment)
