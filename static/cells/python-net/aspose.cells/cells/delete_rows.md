##delete_rows method
## delete_rows(self, row_index, total_rows) {#int-int}
Deletes multiple rows.
```python
def delete_rows(self, row_index, total_rows):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| row_index | int | The first row index to be deleted. |
| total_rows | int | Count of rows to be deleted. |
### Remarks
If the deleted range contains the top part(not whole) of the table(ListObject),
the ranged could not be deleted and nothing will be done.
It works in the same way with MS Excel.
## delete_rows(self, row_index, total_rows, update_reference) {#int-int-bool}
Deletes multiple rows in the worksheet.
### Returns
```python
def delete_rows(self, row_index, total_rows, update_reference):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| row_index | int | Index of the first row to be deleted. |
| total_rows | int | Count of rows to be deleted. |
| update_reference | bool | Indicates whether update references in other worksheets. |
## delete_rows(self, row_index, total_rows, options) {#int-int-aspose.cells.DeleteOptions}
Deletes multiple rows in the worksheet.
### Returns
```python
def delete_rows(self, row_index, total_rows, options):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| row_index | int | Index of the first row to be deleted. |
| total_rows | int | Count of rows to be deleted. |
| options | aspose.cells.DeleteOptions | Options for the deleting operation |
### See Also
* module [`aspose.cells`](../../)
* class [`Cells`](/cells/python-net/aspose.cells/cells)
