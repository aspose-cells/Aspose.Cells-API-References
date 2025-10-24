##add_freeform method
## add_freeform(self, upper_left_row, top, upper_left_column, left, height, width, paths) {#int-int-int-int-int-int-list}
Adds a freeform shape to the worksheet.
### Returns
A freeform shape.
```python
def add_freeform(self, upper_left_row, top, upper_left_column, left, height, width, paths):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| upper_left_row | int | Upper left row index. |
| top | int | Represents the vertical  offset of freeform shape from its left row, in unit of pixel. |
| upper_left_column | int | Upper left column index. |
| left | int | Represents the horizontal offset of freeform shape from its left column, in unit of pixel. |
| height | int | Represents the height of freeform shape, in unit of pixel. |
| width | int | Represents the width of freeform shape, in unit of pixel. |
| paths | list | Represents a user-defined path |
### Remarks
Notice: That the width and height in the parameters can be any positive integer values, not the total width and height of the ShapePath array specified by ’paths'. The relationship between them is a scale-fill relationship, that is, each ShapePath object will be scaled according to the width and height. Therefore, when there are multiple objects in the 'paths', each ShapePath object needs to be designed reasonably to meet expectations. When there is only one ShapePath object and there are no other requirements, passing the object's width and height as parameter values ​​is a good solution.
### Example
```python
from aspose.cells.drawing import ShapePath
# Custom figure
shapePath = ShapePath()
shapePath.move_to(60, 45)
shapePath.arc_to(25, 25, 0, 270)
shapePath.close()
shapePath.move_to(60, 20)
shapePath.line_to(110, 70)
shapePath.line_to(125, 155.5)
shapePath.arc_to(35.5, 35.5, 0, 270)
shapePath.close()
shapePath.move_to(150, 45)
shapePath.arc_to(25, 25, 0, 270)
shapePathW = shapePath.width_pixel
shapePathH = shapePath.height_pixel
shapePath1 = ShapePath()
shapePath1.move_to(0, 0)
shapePath1.cubic_bezier_to(48.24997, 0.6844,                                 96.5, -7.148871,                                 130, 11.517795)
shapePath1.cubic_bezier_to(163.5, 30.18446,                                 182.24997, 75.351,                                 201, 120.517795)
shapePath1.move_to(150, 80)
shapePath1.arc_to(25, 25, 0, 270)
if shapePath1.width_pixel > shapePathW:
shapePathW = shapePath1.width_pixel
if shapePath1.height_pixel > shapePathH:
shapePathH = shapePath1.height_pixel
# Notice: shapePathH and shapePathH can be any positive integer values, here we just simply set them.
# Insert custom figure into worksheet
shapes.add_freeform(1, 0, 1, 0, shapePathH, shapePathW, [shapePath, shapePath1])
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`Shape`](/cells/python-net/aspose.cells.drawing/shape)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
