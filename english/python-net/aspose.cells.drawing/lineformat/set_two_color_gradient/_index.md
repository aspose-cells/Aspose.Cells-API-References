---
title: set_two_color_gradient method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 40
url: /python-net/aspose.cells.drawing/lineformat/set_two_color_gradient/
is_root: false
---

## set_two_color_gradient(color1, color2, style, variant) {#aspose.pydrawing.Color-aspose.pydrawing.Color-GradientStyleType-int}

Sets the specified fill to a two-color gradient.
Only applies for Excel 2007.



```python
def set_two_color_gradient(self, color1, color2, style, variant):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| color1 | aspose.pydrawing.Color | One gradient color. |
| color2 | aspose.pydrawing.Color | Two gradient color. |
| style | [GradientStyleType](/cells/python-net/aspose.cells.drawing/gradientstyletype) | Gradient shading style. |
| variant | int | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |


## set_two_color_gradient(color1, transparency1, color2, transparency2, style, variant) {#aspose.pydrawing.Color-float-aspose.pydrawing.Color-float-GradientStyleType-int}

Sets the specified fill to a two-color gradient.
Only applies for Excel 2007.



```python
def set_two_color_gradient(self, color1, transparency1, color2, transparency2, style, variant):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| color1 | aspose.pydrawing.Color | One gradient color. |
| transparency1 | float | The degree of transparency of the color1 as a value from 0.0 (opaque) through 1.0 (clear). |
| color2 | aspose.pydrawing.Color | Two gradient color. |
| transparency2 | float | The degree of transparency of the color2 as a value from 0.0 (opaque) through 1.0 (clear). |
| style | [GradientStyleType](/cells/python-net/aspose.cells.drawing/gradientstyletype) | Gradient shading style. |
| variant | int | The gradient variant. Can be a value from 1 through 4, corresponding to one of the four variants on the Gradient tab in the Fill Effects dialog box. If style is GradientStyle.FromCenter, the Variant argument can only be 1 or 2. |



### See Also
* module [aspose.cells.drawing](../../)
* class [LineFormat](/cells/python-net/aspose.cells.drawing/lineformat)
