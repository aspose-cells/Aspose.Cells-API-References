---
title: add_text_effect method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 330
url: /python-net/aspose.cells.drawing/shapecollection/add_text_effect/
is_root: false
---

## add_text_effect(effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width) {#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int-int-int}

Inserts a WordArt object.

### Returns 


Returns a Shape object that represents the new WordArt object.


```python
def add_text_effect(self, effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| effect | [MsoPresetTextEffect](/cells/python-net/aspose.cells.drawing/msopresettexteffect) | The mso preset text effect type. |
| text | str | The WordArt text. |
| font_name | str | The font name. |
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


```
from aspose.cells.drawing import MsoPresetTextEffect

# add a WordArt
wordArt1 = shapes.add_text_effect(MsoPresetTextEffect.TEXT_EFFECT10, "WordArt", "arial", 18, False, False, 3, 0, 3, 0, 200, 50)

```



### See Also
* module [aspose.cells.drawing](../../)
* class [ShapeCollection](/cells/python-net/aspose.cells.drawing/shapecollection)
