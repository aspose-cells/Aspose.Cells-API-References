---
title: set_preset_color_gradient method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 30
url: /python-net/aspose.cells.drawing/lineformat/set_preset_color_gradient/
is_root: false
---

## set_preset_color_gradient(preset_color, style, variant) {#GradientPresetType-GradientStyleType-int}

Sets the specified fill to a preset-color gradient.
Only applies for Excel 2007.



```python
def set_preset_color_gradient(self, preset_color, style, variant):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| preset_color | [GradientPresetType](/cells/python-net/aspose.cells.drawing/gradientpresettype) | Preset color type |
| style | [GradientStyleType](/cells/python-net/aspose.cells.drawing/gradientstyletype) | Gradient shading style. |
| variant | int | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |



### See Also
* module [aspose.cells.drawing](../../)
* class [LineFormat](/cells/python-net/aspose.cells.drawing/lineformat)
