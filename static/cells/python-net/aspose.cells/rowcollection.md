##RowCollection class
## RowCollection class
Collects the [`Row`](/cells/python-net/aspose.cells/row) objects that represent the individual rows in a worksheet.
The RowCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [count](/cells/python-net/aspose.cells/rowcollection/count) | Gets the number of rows in this collection. |
Gets a [`Row`](/cells/python-net/aspose.cells/row) object by given row index. The Row object of given row index will be instantiated if it does not exist before.
### Indexer
| Name | Description |
| :- | :- |
| [index] |  |
### Methods
| Method | Description |
| :- | :- |
| [`get_enumerator(self, reversed, sync)`](/cells/python-net/aspose.cells/rowcollection/get_enumerator/#bool-bool) | Gets an enumerator that iterates rows through this collection |
| [`get_row_by_index(self, index)`](/cells/python-net/aspose.cells/rowcollection/get_row_by_index/#int) | Gets the row object by the position in the list. |
| [`clear(self)`](/cells/python-net/aspose.cells/rowcollection/clear/#) | Clear all rows and cells. |
| [`remove_at(self, index)`](/cells/python-net/aspose.cells/rowcollection/remove_at/#int) | Remove the row item at the specified index(position) in this collection. |
### Example
```python
from aspose.cells import Workbook
# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Get first row
row = worksheet.cells.rows[0]
```
### See Also
* module [`aspose.cells`](..)
* class [`Row`](/cells/python-net/aspose.cells/row)
