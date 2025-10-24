##set_column_width method
## set_column_width(self, column, width) {#int-float}
Sets the width of the specified column in normal view.
```python
def set_column_width(self, column, width):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| column | int | Column index. |
| width | float | Width of column in unit of characters.Column width must be between 0 and 255. |
### Remarks
For spreadsheet, column width is measured as the number of characters
of the maximum digit width of the numbers 0~9 as rendered in the normal style's font.
### See Also
* module [`aspose.cells`](../../)
* class [`Cells`](/cells/python-net/aspose.cells/cells)
