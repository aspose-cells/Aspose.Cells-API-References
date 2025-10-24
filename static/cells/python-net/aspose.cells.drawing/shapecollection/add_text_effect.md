##add_text_effect method
## add_text_effect(self, effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width) {#aspose.cells.drawing.MsoPresetTextEffect-System.String-System.String-int-bool-bool-int-int-int-int-int-int}
Inserts a WordArt object.
### Returns
Returns a Shape object that represents the new WordArt object.
```python
def add_text_effect(self, effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| effect | aspose.cells.drawing.MsoPresetTextEffect | The mso preset text effect type. |
| text | System.String | The WordArt text. |
| font_name | System.String | The font name. |
| size | int | The font size |
| font_bold | bool | Indicates whether font is bold. |
| font_italic | bool | Indicates whether font is italic. |
| upper_left_row | int | Upper left row index. |
| top | int | Represents the vertical  offset of shape from its left row, in unit of pixel. |
| upper_left_column | int | Upper left column index. |
| left | int | Represents the horizontal offset of shape from its left column, in unit of pixel. |
| height | int | Represents the height of shape, in unit of pixel. |
| width | int | Represents the width of shape, in unit of pixel. |
### Example
```python
from aspose.cells.drawing import MsoPresetTextEffect
# add a WordArt
wordArt1 = shapes.add_text_effect(MsoPresetTextEffect.TEXT_EFFECT10, "WordArt", "arial", 18, False, False, 3, 0, 3, 0, 200, 50)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`Shape`](/cells/python-net/aspose.cells.drawing/shape)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
