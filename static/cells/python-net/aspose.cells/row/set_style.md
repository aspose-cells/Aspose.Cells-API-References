##set_style method
## set_style(self, style) {#aspose.cells.Style}
Sets the style of this row.
```python
def set_style(self, style):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| style | aspose.cells.Style | the style to be used as the default style for cells in this row. |
### Remarks
This method only sets the given style as the default style for this row,
without changing the style settings for existing cells in this row.
To update style settings of existing cells to the specified style at the same time,
please use [`Row.apply_style`](/cells/python-net/aspose.cells/row/apply_style)
### See Also
* module [`aspose.cells`](../../)
* class [`Row`](/cells/python-net/aspose.cells/row)
