##add_button method
## add_button(self, upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Adds a Button to the worksheet.
### Returns
A Button object.
```python
def add_button(self, upper_left_row, top, upper_left_column, left, height, width):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| top | int | Represents the vertical  offset of Button from its left row, in unit of pixel. |
| upper_left_column | int | Upper left column index. |
| left | int | Represents the horizontal offset of Button from its left column, in unit of pixel. |
| height | int | Represents the height of Button, in unit of pixel. |
| width | int | Represents the width of Button, in unit of pixel. |
### Example
```python
# add a button
button = shapes.add_button(1, 0, 1, 0, 100, 50)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`Button`](/cells/python-net/aspose.cells.drawing/button)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
