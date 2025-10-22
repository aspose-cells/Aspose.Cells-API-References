##get_locked_property method
## get_locked_property(self, type) {#aspose.cells.drawing.ShapeLockType}
Gets the value of locked property.
### Returns
Returns  the value of locked property.
```python
def get_locked_property(self, type):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| type | aspose.cells.drawing.ShapeLockType | The type of the shape locked property. |
### Example
```python
from aspose.cells.drawing import ShapeLockType
noAdjustHandles = 0
if shape.get_locked_property(ShapeLockType.ADJUST_HANDLES):
noAdjustHandles = 1
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`GroupShape`](/cells/python-net/aspose.cells.drawing/groupshape)
