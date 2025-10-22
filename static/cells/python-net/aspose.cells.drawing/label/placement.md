##placement property
## placement property
Represents the way the drawing object is attached to the cells below it.
The property controls the placement of an object on a worksheet.
### Example
```python
from aspose.cells.drawing import PlacementType
if shape.placement == PlacementType.MOVE:
shape.placement = PlacementType.MOVE_AND_SIZE
```
### Definition:
```python
@property
def placement(self):
...
@placement.setter
def placement(self, value):
...
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`Label`](/cells/python-net/aspose.cells.drawing/label)
* class [`PlacementType`](/cells/python-net/aspose.cells.drawing/placementtype)
