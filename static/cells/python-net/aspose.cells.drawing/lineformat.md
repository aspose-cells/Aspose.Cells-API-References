##LineFormat class
## LineFormat class
Represents all setting of the line.
**Inheritance:** [`LineFormat`](/cells/python-net/aspose.cells.drawing/lineformat) →
[`FillFormat`](/cells/python-net/aspose.cells.drawing/fillformat)
The LineFormat type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [type](/cells/python-net/aspose.cells.drawing/lineformat/type) | Gets and sets the fill type. |
| [fill_type](/cells/python-net/aspose.cells.drawing/lineformat/fill_type) | Gets and sets fill type |
| [transparency](/cells/python-net/aspose.cells.drawing/lineformat/transparency) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [set_type](/cells/python-net/aspose.cells.drawing/lineformat/set_type) | Gets the fill format set type. |
| [gradient_fill](/cells/python-net/aspose.cells.drawing/lineformat/gradient_fill) | Gets [`FillFormat.gradient_fill`](/cells/python-net/aspose.cells.drawing/fillformat#gradient_fill) object. |
| [texture_fill](/cells/python-net/aspose.cells.drawing/lineformat/texture_fill) | Gets [`FillFormat.texture_fill`](/cells/python-net/aspose.cells.drawing/fillformat#texture_fill) object. |
| [solid_fill](/cells/python-net/aspose.cells.drawing/lineformat/solid_fill) | Gets [`FillFormat.solid_fill`](/cells/python-net/aspose.cells.drawing/fillformat#solid_fill) object. |
| [pattern_fill](/cells/python-net/aspose.cells.drawing/lineformat/pattern_fill) | Gets [`FillFormat.pattern_fill`](/cells/python-net/aspose.cells.drawing/fillformat#pattern_fill) object. |
| [gradient_color_type](/cells/python-net/aspose.cells.drawing/lineformat/gradient_color_type) | Returns the gradient color type for the specified fill. |
| [gradient_style](/cells/python-net/aspose.cells.drawing/lineformat/gradient_style) | Returns the gradient style for the specified fill. |
| [gradient_color1](/cells/python-net/aspose.cells.drawing/lineformat/gradient_color1) | Returns the gradient color 1 for the specified fill. |
| [gradient_color2](/cells/python-net/aspose.cells.drawing/lineformat/gradient_color2) | Returns the gradient color 2 for the specified fill. |
| [gradient_degree](/cells/python-net/aspose.cells.drawing/lineformat/gradient_degree) | Returns the gradient degree for the specified fill.
| [gradient_variant](/cells/python-net/aspose.cells.drawing/lineformat/gradient_variant) | Returns the gradient variant for the specified fill.
| [preset_color](/cells/python-net/aspose.cells.drawing/lineformat/preset_color) | Returns the gradient preset color for the specified fill. |
| [texture](/cells/python-net/aspose.cells.drawing/lineformat/texture) | Represents the texture type for the specified fill. |
| [pattern](/cells/python-net/aspose.cells.drawing/lineformat/pattern) | Represents an area's display pattern. |
| [picture_format_type](/cells/python-net/aspose.cells.drawing/lineformat/picture_format_type) | Gets and sets the picture format type. |
| [scale](/cells/python-net/aspose.cells.drawing/lineformat/scale) | Gets and sets the picture format scale. |
| [image_data](/cells/python-net/aspose.cells.drawing/lineformat/image_data) | Gets and sets the picture image data. |
| [compound_type](/cells/python-net/aspose.cells.drawing/lineformat/compound_type) | Specifies the line compound type. |
| [dash_style](/cells/python-net/aspose.cells.drawing/lineformat/dash_style) | Specifies the line dash type. |
| [cap_type](/cells/python-net/aspose.cells.drawing/lineformat/cap_type) | Specifies the ending caps. |
| [join_type](/cells/python-net/aspose.cells.drawing/lineformat/join_type) | Specifies the line join type. |
| [begin_arrowhead_style](/cells/python-net/aspose.cells.drawing/lineformat/begin_arrowhead_style) | Gets and sets the begin arrow type of the line. |
| [begin_arrowhead_width](/cells/python-net/aspose.cells.drawing/lineformat/begin_arrowhead_width) | Gets and sets the begin arrow width type of the line. |
| [begin_arrowhead_length](/cells/python-net/aspose.cells.drawing/lineformat/begin_arrowhead_length) | Gets and sets the begin arrow length type of the line. |
| [end_arrowhead_style](/cells/python-net/aspose.cells.drawing/lineformat/end_arrowhead_style) | Gets and sets the end arrow type of the line. |
| [end_arrowhead_width](/cells/python-net/aspose.cells.drawing/lineformat/end_arrowhead_width) | Gets and sets the end arrow width type of the line. |
| [end_arrowhead_length](/cells/python-net/aspose.cells.drawing/lineformat/end_arrowhead_length) | Gets and sets the end arrow length type of the line. |
| [weight](/cells/python-net/aspose.cells.drawing/lineformat/weight) | Gets or sets the weight of the line in unit of points. |
### Methods
| Method | Description |
| :- | :- |
| [`set_two_color_gradient(self, color1, color2, style, variant)`](/cells/python-net/aspose.cells.drawing/lineformat/set_two_color_gradient/#aspose.pydrawing.color-aspose.pydrawing.color-aspose.cells.drawing.gradientstyletype-int) | Sets the specified fill to a two-color gradient.
| [`set_two_color_gradient(self, color1, transparency1, color2, transparency2, style, variant)`](/cells/python-net/aspose.cells.drawing/lineformat/set_two_color_gradient/#aspose.pydrawing.color-float-aspose.pydrawing.color-float-aspose.cells.drawing.gradientstyletype-int) | Sets the specified fill to a two-color gradient.
| [`set_one_color_gradient(self, color, degree, style, variant)`](/cells/python-net/aspose.cells.drawing/lineformat/set_one_color_gradient/#aspose.pydrawing.color-float-aspose.cells.drawing.gradientstyletype-int) | Sets the specified fill to a one-color gradient.
| [`set_preset_color_gradient(self, preset_color, style, variant)`](/cells/python-net/aspose.cells.drawing/lineformat/set_preset_color_gradient/#aspose.cells.drawing.gradientpresettype-aspose.cells.drawing.gradientstyletype-int) | Sets the specified fill to a preset-color gradient.
### Example
```python
from aspose.cells import Workbook
# Instantiating a Workbook object
workbook = Workbook()
shapes = workbook.worksheets[0].shapes
shape = shapes.add_rectangle(1, 0, 1, 0, 50, 100)
lineFmt = shape.line
```
### See Also
* module [`aspose.cells.drawing`](..)
* class [`FillFormat`](/cells/python-net/aspose.cells.drawing/fillformat)
* class [`LineFormat`](/cells/python-net/aspose.cells.drawing/lineformat)
