##create_range method
## create_range(self, address) {#System.String}
Creates a [`Range`](/cells/python-net/aspose.cells/range) object from an address of the range.
### Returns
A [`Range`](/cells/python-net/aspose.cells/range) object
```python
def create_range(self, address):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| address | System.String | The address of the range. |
## create_range(self, upper_left_cell, lower_right_cell) {#System.String-System.String}
Creates a [`Range`](/cells/python-net/aspose.cells/range) object from a range of cells.
### Returns
A [`Range`](/cells/python-net/aspose.cells/range) object
```python
def create_range(self, upper_left_cell, lower_right_cell):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_cell | System.String | Upper left cell name. |
| lower_right_cell | System.String | Lower right cell name. |
## create_range(self, first_index, number, is_vertical) {#int-int-bool}
Creates a [`Range`](/cells/python-net/aspose.cells/range) object from rows of cells or columns of cells.
### Returns
A [`Range`](/cells/python-net/aspose.cells/range) object.
```python
def create_range(self, first_index, number, is_vertical):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| first_index | int | First row index or first column index, zero based. |
| number | int | Total number of rows or columns, one based. |
| is_vertical | bool | True - Range created from columns of cells. False - Range created from rows of cells. |
## create_range(self, first_row, first_column, total_rows, total_columns) {#int-int-int-int}
Creates a [`Range`](/cells/python-net/aspose.cells/range) object from a range of cells.
### Returns
A [`Range`](/cells/python-net/aspose.cells/range) object
```python
def create_range(self, first_row, first_column, total_rows, total_columns):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| first_row | int | First row of this range |
| first_column | int | First column of this range |
| total_rows | int | Number of rows |
| total_columns | int | Number of columns |
### See Also
* module [`aspose.cells`](../../)
* class [`Cells`](/cells/python-net/aspose.cells/cells)
* class [`Range`](/cells/python-net/aspose.cells/range)
