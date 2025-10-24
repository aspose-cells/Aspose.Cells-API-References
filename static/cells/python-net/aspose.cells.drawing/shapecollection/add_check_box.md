##add_check_box method
## add_check_box(self, upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Adds a checkbox to the worksheet.
### Returns
The new CheckBox object index.
```python
def add_check_box(self, upper_left_row, top, upper_left_column, left, height, width):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| top | int | Represents the vertical  offset of checkbox from its top row, in unit of pixel. |
| upper_left_column | int | Upper left column index. |
| left | int | Represents the horizontal offset of textbox from its left column, in unit of pixel. |
| height | int | Height of textbox, in unit of pixel. |
| width | int | Width of textbox, in unit of pixel. |
### Example
```python
# add a CheckBox
checkBox = shapes.add_check_box(1, 0, 1, 0, 100, 50)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`CheckBox`](/cells/python-net/aspose.cells.drawing/checkbox)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
