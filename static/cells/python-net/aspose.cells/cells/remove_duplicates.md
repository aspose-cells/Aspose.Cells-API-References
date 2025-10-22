##remove_duplicates method
## remove_duplicates(self) {#}
Removes duplicate rows in the sheet.
```python
def remove_duplicates(self):
...
```
## remove_duplicates(self, start_row, start_column, end_row, end_column) {#int-int-int-int}
Removes duplicate values in the range.
```python
def remove_duplicates(self, start_row, start_column, end_row, end_column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| start_row | int | The start row. |
| start_column | int | The start column |
| end_row | int | The end row index. |
| end_column | int | The end column index. |
## remove_duplicates(self, start_row, start_column, end_row, end_column, has_headers, column_offsets) {#int-int-int-int-bool-list}
Removes duplicate data of the range.
```python
def remove_duplicates(self, start_row, start_column, end_row, end_column, has_headers, column_offsets):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| start_row | int | The start row. |
| start_column | int | The start column |
| end_row | int | The end row index. |
| end_column | int | The end column index. |
| has_headers | bool | Indicates whether the range contains headers. |
| column_offsets | list | The column offsets. |
### See Also
* module [`aspose.cells`](../../)
* class [`Cells`](/cells/python-net/aspose.cells/cells)
