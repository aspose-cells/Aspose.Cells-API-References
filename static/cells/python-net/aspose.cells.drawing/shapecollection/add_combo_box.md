##add_combo_box method
## add_combo_box(self, upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Adds a ComboBox to the worksheet.
### Returns
A ComboBox object.
```python
def add_combo_box(self, upper_left_row, top, upper_left_column, left, height, width):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| top | int | Represents the vertical  offset of ComboBox from its left row, in unit of pixel. |
| upper_left_column | int | Upper left column index. |
| left | int | Represents the horizontal offset of ComboBox from its left column, in unit of pixel. |
| height | int | Represents the height of ComboBox, in unit of pixel. |
| width | int | Represents the width of ComboBox, in unit of pixel. |
### Example
```python
# add a combo box
comboBox = shapes.add_combo_box(1, 0, 1, 0, 100, 50)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`ComboBox`](/cells/python-net/aspose.cells.drawing/combobox)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
