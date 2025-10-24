##sort method
## sort(self) {#}
Sort the data in the range.
### Returns
the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns.
If no rows/columns needs to be moved by this sorting operation, null will be returned.
```python
def sort(self):
...
```
## sort(self, cells, area) {#aspose.cells.Cells-aspose.cells.CellArea}
Sort the data of the area.
### Returns
the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns.
If no rows/columns needs to be moved by this sorting operation, null will be returned.
```python
def sort(self, cells, area):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| cells | aspose.cells.Cells | The cells contains the data area. |
| area | aspose.cells.CellArea | The area needed to sort |
## sort(self, cells, start_row, start_column, end_row, end_column) {#aspose.cells.Cells-int-int-int-int}
Sorts the data of the area.
### Returns
the original indices(absolute position, for example, column A is 0, B is 1, ...) of the sorted rows/columns.
If no rows/columns needs to be moved by this sorting operation, null will be returned.
```python
def sort(self, cells, start_row, start_column, end_row, end_column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| cells | aspose.cells.Cells | The cells contains the data area. |
| start_row | int | The start row of the area. |
| start_column | int | The start column of the area. |
| end_row | int | The end row of the area. |
| end_column | int | The end column of the area. |
### See Also
* module [`aspose.cells`](../../)
* class [`DataSorter`](/cells/python-net/aspose.cells/datasorter)
