##add_arc method
## add_arc(self, upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Adds a ArcShape to the worksheet.
### Returns
A ArcShape object.
```python
def add_arc(self, upper_left_row, top, upper_left_column, left, height, width):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| top | int | Represents the vertical  offset of ArcShape from its left row, in unit of pixel. |
| upper_left_column | int | Upper left column index. |
| left | int | Represents the horizontal offset of ArcShape from its left column, in unit of pixel. |
| height | int | Represents the height of ArcShape, in unit of pixel. |
| width | int | Represents the width of ArcShape, in unit of pixel. |
### Example
```python
# add a arc
arcShape = shapes.add_arc(1, 0, 1, 0, 100, 50)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`ArcShape`](/cells/python-net/aspose.cells.drawing/arcshape)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
