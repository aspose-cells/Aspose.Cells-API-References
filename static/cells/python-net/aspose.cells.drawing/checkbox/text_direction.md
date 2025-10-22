##text_direction property
## text_direction property
Gets/Sets the direction of the text flow for this object.
### Example
```python
from aspose.cells import TextDirectionType
if shape.text_direction == TextDirectionType.CONTEXT:
shape.text_direction = TextDirectionType.LEFT_TO_RIGHT
```
### Definition:
```python
@property
def text_direction(self):
...
@text_direction.setter
def text_direction(self, value):
...
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`CheckBox`](/cells/python-net/aspose.cells.drawing/checkbox)
* class [`TextDirectionType`](/cells/python-net/aspose.cells/textdirectiontype)
