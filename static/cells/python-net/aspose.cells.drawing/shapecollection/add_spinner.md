##add_spinner method
## add_spinner(self, upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Adds a Spinner to the worksheet.
### Returns
A Spinner object.
```python
def add_spinner(self, upper_left_row, top, upper_left_column, left, height, width):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| top | int | Represents the vertical  offset of Spinner from its left row, in unit of pixel. |
| upper_left_column | int | Upper left column index. |
| left | int | Represents the horizontal offset of Spinner from its left column, in unit of pixel. |
| height | int | Represents the height of Spinner, in unit of pixel. |
| width | int | Represents the width of Spinner, in unit of pixel. |
### Example
```python
# add a spinner
spinner = shapes.add_spinner(1, 0, 1, 0, 100, 50)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
* class [`Spinner`](/cells/python-net/aspose.cells.drawing/spinner)
