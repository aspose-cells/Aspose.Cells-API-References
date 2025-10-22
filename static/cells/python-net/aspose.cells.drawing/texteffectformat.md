##TextEffectFormat class
## TextEffectFormat class
Contains properties and methods that apply to WordArt objects.
The TextEffectFormat type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [text](/cells/python-net/aspose.cells.drawing/texteffectformat/text) | The text in the WordArt. |
| [font_name](/cells/python-net/aspose.cells.drawing/texteffectformat/font_name) | The name of the font used in the WordArt. |
| [font_bold](/cells/python-net/aspose.cells.drawing/texteffectformat/font_bold) | Indicates whether font is bold. |
| [font_italic](/cells/python-net/aspose.cells.drawing/texteffectformat/font_italic) | Indicates whether font is italic. |
| [rotated_chars](/cells/python-net/aspose.cells.drawing/texteffectformat/rotated_chars) | If true,characters in the specified WordArt are rotated 90 degrees relative to the WordArt's bounding shape. |
| [font_size](/cells/python-net/aspose.cells.drawing/texteffectformat/font_size) | The size (in points) of the font used in the WordArt. |
| [preset_shape](/cells/python-net/aspose.cells.drawing/texteffectformat/preset_shape) | Gets and sets the preset shape type. |
### Methods
| Method | Description |
| :- | :- |
| [`set_text_effect(self, effect)`](/cells/python-net/aspose.cells.drawing/texteffectformat/set_text_effect/#aspose.cells.drawing.msopresettexteffect) | Sets the preset text effect. |
### Example
```python
from aspose.cells import Workbook
from aspose.cells.drawing import MsoPresetTextEffect
# Instantiating a Workbook object
workbook = Workbook()
shapes = workbook.worksheets[0].shapes
shapes.add_text_effect(MsoPresetTextEffect.TEXT_EFFECT1, "Aspose", "Arial", 30, False, False, 0, 0, 0, 0, 100, 200)
textEffectFormat = shapes[0].text_effect
textEffectFormat.set_text_effect(MsoPresetTextEffect.TEXT_EFFECT10)
workbook.save("Book1.xls")
```
### See Also
* module [`aspose.cells.drawing`](..)
