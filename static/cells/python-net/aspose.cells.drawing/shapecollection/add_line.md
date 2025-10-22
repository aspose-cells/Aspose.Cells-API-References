##add_line method
## add_line(self, upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Adds a LineShape to the worksheet.
### Returns
A LineShape object.
```python
def add_line(self, upper_left_row, top, upper_left_column, left, height, width):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| top | int | Represents the vertical  offset of LineShape from its left row, in unit of pixel. |
| upper_left_column | int | Upper left column index. |
| left | int | Represents the horizontal offset of LineShape from its left column, in unit of pixel. |
| height | int | Represents the height of LineShape, in unit of pixel. |
| width | int | Represents the width of LineShape, in unit of pixel. |
### Example
```python
#  add a line object
lineShape = shapes.add_line(1, 0, 1, 0, 100, 50)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`LineShape`](/cells/python-net/aspose.cells.drawing/lineshape)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
