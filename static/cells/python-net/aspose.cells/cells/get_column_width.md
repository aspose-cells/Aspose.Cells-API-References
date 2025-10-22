##get_column_width method
## get_column_width(self, column) {#int}
Gets the width(in unit of characters) of the specified column in normal view
### Returns
Width of column. For spreadsheet, column width is measured as the number of characters
of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.
```python
def get_column_width(self, column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| column | int | Column index |
## get_column_width(self, column, is_original, unit_type) {#int-bool-aspose.cells.CellsUnitType}
Gets the column width.
### Returns
```python
def get_column_width(self, column, is_original, unit_type):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| column | int | The column index. |
| is_original | bool | Indicates whether getting original width. |
| unit_type | aspose.cells.CellsUnitType |  |
### See Also
* module [`aspose.cells`](../../)
* class [`Cells`](/cells/python-net/aspose.cells/cells)
