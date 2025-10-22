##add_word_art method
## add_word_art(self, style, text, upper_left_row, top, upper_left_column, left, height, width) {#aspose.cells.drawing.PresetWordArtStyle-System.String-int-int-int-int-int-int}
Adds preset WordArt since Excel 2007.s
### Returns
```python
def add_word_art(self, style, text, upper_left_row, top, upper_left_column, left, height, width):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| style | aspose.cells.drawing.PresetWordArtStyle | The preset WordArt Style. |
| text | System.String | The text. |
| upper_left_row | int | Upper left row index. |
| top | int | Represents the vertical  offset of shape from its left row, in unit of pixel. |
| upper_left_column | int | Upper left column index. |
| left | int | Represents the horizontal offset of shape from its left column, in unit of pixel. |
| height | int | Represents the height of shape, in unit of pixel. |
| width | int | Represents the width of shape, in unit of pixel. |
### Example
```python
from aspose.cells.drawing import PresetWordArtStyle
# add a WordArt
wordArt2 = shapes.add_word_art(PresetWordArtStyle.WORD_ART_STYLE1, "WordArt", 3, 0, 3, 0, 50, 200)
```
### See Also
* module [`aspose.cells.drawing`](../../)
* class [`Shape`](/cells/python-net/aspose.cells.drawing/shape)
* class [`ShapeCollection`](/cells/python-net/aspose.cells.drawing/shapecollection)
