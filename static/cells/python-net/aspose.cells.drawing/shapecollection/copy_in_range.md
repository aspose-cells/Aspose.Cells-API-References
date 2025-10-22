##copy_in_range method
## copy_in_range(self, source_shapes, ca, dest_row, dest_column, is_contained) {#aspose.cells.drawing.ShapeCollection-aspose.cells.CellArea-int-int-bool}
Copy shapes in the range to destination range.
```python
def copy_in_range(self, source_shapes, ca, dest_row, dest_column, is_contained):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| source_shapes | aspose.cells.drawing.ShapeCollection | Source shapes. |
| ca | aspose.cells.CellArea | The source range. |
| dest_row | int | The dest row index of the dest range. |
| dest_column | int | The dest column of the dest range. |
| is_contained | bool | Whether only copy the shapes which are contained in the range.
### Example
```python
from aspose.cells import CellArea
# add a shape
shapes.add_rectangle(2, 0, 2, 0, 130, 130)
area2 = CellArea()
area2.start_column = 1
area2.start_row = 1
area2.end_column = 5
area2.end_row = 11
# copy
shapes.copy_in_range(shapes, area2, 12, 1, False)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
