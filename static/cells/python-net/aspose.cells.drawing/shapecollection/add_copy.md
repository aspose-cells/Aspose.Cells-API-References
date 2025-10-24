##add_copy method
## add_copy(self, source_shape, top_row, top, left_column, left) {#aspose.cells.drawing.Shape-int-int-int-int}
Adds and copy a shape to the worksheet.
### Returns
The new [`Shape`](/cells/python-net/aspose.cells.drawing/shape) object.
```python
def add_copy(self, source_shape, top_row, top, left_column, left):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| source_shape | aspose.cells.drawing.Shape | Source shape. |
| top_row | int | The top row index. |
| top | int | Represents the vertical  offset from its top row, in unit of pixel. |
| left_column | int | The left column index. |
| left | int | Represents the horizontal offset from its left column, in unit of pixel. |
### Example
```python
# add a shape
rectangle = shapes.add_rectangle(2, 0, 2, 0, 130, 130)
# Adds and copies a shape.
shapes.add_copy(rectangle, 7, 0, 7, 0)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`Shape`](/cells/python-net/aspose.cells.drawing/shape)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
