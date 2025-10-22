##text_horizontal_overflow property
## text_horizontal_overflow property
Gets and sets the text horizontal overflow type of the shape which contains text.
### Example
```python
from aspose.cells.drawing import TextOverflowType
if shape.text_horizontal_overflow == TextOverflowType.CLIP:
shape.text_horizontal_overflow = TextOverflowType.OVERFLOW
```
### Definition:
```python
@property
def text_horizontal_overflow(self):
...
@text_horizontal_overflow.setter
def text_horizontal_overflow(self, value):
...
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`CellsDrawing`](/cells/python-net/aspose.cells.drawing/cellsdrawing)
* class [`TextOverflowType`](/cells/python-net/aspose.cells.drawing/textoverflowtype)
