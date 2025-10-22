##add_radio_button method
## add_radio_button(self, upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Adds a RadioButton to the worksheet.
### Returns
A RadioButton object.
```python
def add_radio_button(self, upper_left_row, top, upper_left_column, left, height, width):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| top | int | Represents the vertical  offset of RadioButton from its left row, in unit of pixel. |
| upper_left_column | int | Upper left column index. |
| left | int | Represents the horizontal offset of RadioButton from its left column, in unit of pixel. |
| height | int | Represents the height of RadioButton, in unit of pixel. |
| width | int | Represents the width of RadioButton, in unit of pixel. |
### Example
```python
# add a radio button
radioButton = shapes.add_radio_button(1, 0, 1, 0, 100, 50)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`RadioButton`](/cells/python-net/aspose.cells.drawing/radiobutton)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
