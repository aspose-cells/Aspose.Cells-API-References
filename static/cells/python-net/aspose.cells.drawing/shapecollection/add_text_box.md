##add_text_box method
## add_text_box(self, upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Adds a text box to the worksheet.
### Returns
A [`TextBox`](/cells/python-net/aspose.cells.drawing/textbox) object.
```python
def add_text_box(self, upper_left_row, top, upper_left_column, left, height, width):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| top | int | Represents the vertical  offset of textbox from its top row, in unit of pixel. |
| upper_left_column | int | Upper left column index. |
| left | int | Represents the horizontal offset of textbox from its left column, in unit of pixel. |
| height | int | Represents the height of textbox, in unit of pixel. |
| width | int | Represents the width of textbox, in unit of pixel. |
### Example
```python
# add a TextBox
textBox = shapes.add_text_box(1, 0, 1, 0, 100, 50)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
* class [`TextBox`](/cells/python-net/aspose.cells.drawing/textbox)
