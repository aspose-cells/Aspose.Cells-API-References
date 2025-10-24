##add_auto_shape method
## add_auto_shape(self, type, upper_left_row, top, upper_left_column, left, height, width) {#aspose.cells.drawing.AutoShapeType-int-int-int-int-int-int}
Adds a AutoShape to the worksheet.
### Returns
A Shape object.
```python
def add_auto_shape(self, type, upper_left_row, top, upper_left_column, left, height, width):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| type | aspose.cells.drawing.AutoShapeType | Auto shape type. |
| upper_left_row | int | Upper left row index. |
| top | int | Represents the vertical  offset of Shape from its left row, in unit of pixel. |
| upper_left_column | int | Upper left column index. |
| left | int | Represents the horizontal offset of Shape from its left column, in unit of pixel. |
| height | int | Represents the height of Shape, in unit of pixel. |
| width | int | Represents the width of Shape, in unit of pixel. |
### Remarks
The type could not be Chart/Comment/Picture/OleObject/Polygon/DialogBox
### Example
```python
from aspose.cells.drawing import AutoShapeType
# Adds a AutoShape to the worksheet.
autoShape = shapes.add_auto_shape(AutoShapeType.CUBE, 1, 0, 1, 0, 100, 50)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`Shape`](/cells/python-net/aspose.cells.drawing/shape)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
