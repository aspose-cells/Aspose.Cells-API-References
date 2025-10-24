##get_cell_display_style method
## get_cell_display_style(self, row, column) {#int-int}
Get the display style of given cell.
### Returns
the display style of given cell.
```python
def get_cell_display_style(self, row, column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| row | int | row index of given cell |
| column | int | column of given cell |
### Remarks
Same with [`Cell.get_display_style`](/cells/python-net/aspose.cells/cell/get_display_style),
and same with using [`BorderType.SIDE_BORDERS`](/cells/python-net/aspose.cells/bordertype#SIDE_BORDERS)
for [`Cells.get_cell_display_style`](/cells/python-net/aspose.cells/cells/get_cell_display_style).
## get_cell_display_style(self, row, column, adjacent_borders) {#int-int-aspose.cells.BorderType}
Get the display style of given cell.
### Returns
the display style of given cell.
```python
def get_cell_display_style(self, row, column, adjacent_borders):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| row | int | row index of given cell |
| column | int | column of given cell |
| adjacent_borders | aspose.cells.BorderType | Indicates which borders need to be checked and adjusted according to the borders of adjacent cells.
### Remarks
If the cell is also affected by other settings such as conditional formatting, list objects, etc.,
then the display style may be different from [`Cells.get_cell_style`](/cells/python-net/aspose.cells/cells/get_cell_style).
And because those settings also may be applied to empty(non-existing) cells,
using this method can avoid the instantiation of those empty cells
so the performance will be better than getting the Cell instance from Cells
and then calling [`Cell.get_display_style`](/cells/python-net/aspose.cells/cell/get_display_style).
### See Also
* module [`aspose.cells`](../../)
* class [`Cells`](/cells/python-net/aspose.cells/cells)
* class [`Style`](/cells/python-net/aspose.cells/style)
