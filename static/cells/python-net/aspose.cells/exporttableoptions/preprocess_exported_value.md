##preprocess_exported_value method
## preprocess_exported_value(self, cell_row, cell_column, value) {#int-int-aspose.cells.CellValue}
Preprocess the value of current cell to be exported.
### Returns
Whether current cell has been replaced with different type and/or value.
```python
def preprocess_exported_value(self, cell_row, cell_column, value):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| cell_row | int | the row index of current cell |
| cell_column | int | the column index of cell |
| value | aspose.cells.CellValue | value and type of current cell |
### Remarks
The row and column index is cell's absolute index in the worksheet, not index in the exported table.
User may check the value of current cell in the override implementation of this method,
if current cell needs to be replaced with other type and value,
here the implementation should set the expected type and value to the CellValue object and return true.
By default this method does nothing and returns false.
### See Also
* module [`aspose.cells`](../../)
* class [`ExportTableOptions`](/cells/python-net/aspose.cells/exporttableoptions)
