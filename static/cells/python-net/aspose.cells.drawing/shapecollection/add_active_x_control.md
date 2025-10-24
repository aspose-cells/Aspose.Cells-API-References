##add_active_x_control method
## add_active_x_control(self, type, top_row, top, left_column, left, width, height) {#aspose.cells.drawing.activexcontrols.ControlType-int-int-int-int-int-int}
Creates an Activex Control.
### Returns
```python
def add_active_x_control(self, type, top_row, top, left_column, left, width, height):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| type | aspose.cells.drawing.activexcontrols.ControlType | The type of the control. |
| top_row | int | Upper left row index. |
| top | int | Represents the vertical  offset of Shape from its left row, in unit of pixel. |
| left_column | int | Upper left column index. |
| left | int | Represents the horizontal offset of Shape from its left column, in unit of pixel. |
| width | int | Represents the width of Shape, in unit of pixel. |
| height | int | Represents the height of Shape, in unit of pixel. |
### Example
```python
from aspose.cells.drawing.activexcontrols import ControlType
# add an ActiveX control
activeXControl = shapes.add_active_x_control(ControlType.CHECK_BOX, 1, 0, 1, 0, 100, 50)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`Shape`](/cells/python-net/aspose.cells.drawing/shape)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
