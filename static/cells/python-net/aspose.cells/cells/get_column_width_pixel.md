##get_column_width_pixel method
## get_column_width_pixel(self, column) {#int}
Gets the width of the specified column in normal view, in units of pixel.
### Returns
Width of column in normal view.
```python
def get_column_width_pixel(self, column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| column | int | Column index |
## get_column_width_pixel(self, column, original) {#int-bool}
Gets the width of the specified column in normal view, in units of pixel.
### Returns
Width of column in normal view.
```python
def get_column_width_pixel(self, column, original):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| column | int | Column index |
| original | bool | Indicates whether returning original width even when the column is hidden |
### Remarks
NOTE: This method is now obsolete. Instead,
please use Cells.GetColumnWidth(int ,bool , CellsUnitType ) method.
This method will be removed 12 months later since April 2024.
Aspose apologizes for any inconvenience you may have experienced.
### See Also
* module [`aspose.cells`](../../)
* class [`Cells`](/cells/python-net/aspose.cells/cells)
