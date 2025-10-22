##FillFormat class
## FillFormat class
Encapsulates the object that represents fill formatting for a shape.
The FillFormat type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [type](/cells/python-net/aspose.cells.drawing/fillformat/type) | Gets and sets the fill type. |
| [fill_type](/cells/python-net/aspose.cells.drawing/fillformat/fill_type) | Gets and sets fill type |
| [transparency](/cells/python-net/aspose.cells.drawing/fillformat/transparency) | Returns or sets the degree of transparency of the area as a value from 0.0 (opaque) through 1.0 (clear). |
| [set_type](/cells/python-net/aspose.cells.drawing/fillformat/set_type) | Gets the fill format set type. |
| [gradient_fill](/cells/python-net/aspose.cells.drawing/fillformat/gradient_fill) | Gets [`FillFormat.gradient_fill`](/cells/python-net/aspose.cells.drawing/fillformat#gradient_fill) object. |
| [texture_fill](/cells/python-net/aspose.cells.drawing/fillformat/texture_fill) | Gets [`FillFormat.texture_fill`](/cells/python-net/aspose.cells.drawing/fillformat#texture_fill) object. |
| [solid_fill](/cells/python-net/aspose.cells.drawing/fillformat/solid_fill) | Gets [`FillFormat.solid_fill`](/cells/python-net/aspose.cells.drawing/fillformat#solid_fill) object. |
| [pattern_fill](/cells/python-net/aspose.cells.drawing/fillformat/pattern_fill) | Gets [`FillFormat.pattern_fill`](/cells/python-net/aspose.cells.drawing/fillformat#pattern_fill) object. |
| [gradient_color_type](/cells/python-net/aspose.cells.drawing/fillformat/gradient_color_type) | Returns the gradient color type for the specified fill. |
| [gradient_style](/cells/python-net/aspose.cells.drawing/fillformat/gradient_style) | Returns the gradient style for the specified fill. |
| [gradient_color1](/cells/python-net/aspose.cells.drawing/fillformat/gradient_color1) | Returns the gradient color 1 for the specified fill. |
| [gradient_color2](/cells/python-net/aspose.cells.drawing/fillformat/gradient_color2) | Returns the gradient color 2 for the specified fill. |
| [gradient_degree](/cells/python-net/aspose.cells.drawing/fillformat/gradient_degree) | Returns the gradient degree for the specified fill.
| [gradient_variant](/cells/python-net/aspose.cells.drawing/fillformat/gradient_variant) | Returns the gradient variant for the specified fill.
| [preset_color](/cells/python-net/aspose.cells.drawing/fillformat/preset_color) | Returns the gradient preset color for the specified fill. |
| [texture](/cells/python-net/aspose.cells.drawing/fillformat/texture) | Represents the texture type for the specified fill. |
| [pattern](/cells/python-net/aspose.cells.drawing/fillformat/pattern) | Represents an area's display pattern. |
| [picture_format_type](/cells/python-net/aspose.cells.drawing/fillformat/picture_format_type) | Gets and sets the picture format type. |
| [scale](/cells/python-net/aspose.cells.drawing/fillformat/scale) | Gets and sets the picture format scale. |
| [image_data](/cells/python-net/aspose.cells.drawing/fillformat/image_data) | Gets and sets the picture image data. |
### Methods
| Method | Description |
| :- | :- |
| [`set_two_color_gradient(self, color1, color2, style, variant)`](/cells/python-net/aspose.cells.drawing/fillformat/set_two_color_gradient/#aspose.pydrawing.color-aspose.pydrawing.color-aspose.cells.drawing.gradientstyletype-int) | Sets the specified fill to a two-color gradient.
| [`set_two_color_gradient(self, color1, transparency1, color2, transparency2, style, variant)`](/cells/python-net/aspose.cells.drawing/fillformat/set_two_color_gradient/#aspose.pydrawing.color-float-aspose.pydrawing.color-float-aspose.cells.drawing.gradientstyletype-int) | Sets the specified fill to a two-color gradient.
| [`set_one_color_gradient(self, color, degree, style, variant)`](/cells/python-net/aspose.cells.drawing/fillformat/set_one_color_gradient/#aspose.pydrawing.color-float-aspose.cells.drawing.gradientstyletype-int) | Sets the specified fill to a one-color gradient.
| [`set_preset_color_gradient(self, preset_color, style, variant)`](/cells/python-net/aspose.cells.drawing/fillformat/set_preset_color_gradient/#aspose.cells.drawing.gradientpresettype-aspose.cells.drawing.gradientstyletype-int) | Sets the specified fill to a preset-color gradient.
### Example
```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType
from aspose.cells.drawing import GradientStyleType
from aspose.pydrawing import Color
# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Excel object
sheetIndex = workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[sheetIndex]
# Adding a sample value to "A1" cell
worksheet.cells.get("A1").put_value(50)
# Adding a sample value to "A2" cell
worksheet.cells.get("A2").put_value(100)
# Adding a sample value to "A3" cell
worksheet.cells.get("A3").put_value(150)
# Adding a sample value to "A4" cell
worksheet.cells.get("A4").put_value(200)
# Adding a sample value to "B1" cell
worksheet.cells.get("B1").put_value(60)
# Adding a sample value to "B2" cell
worksheet.cells.get("B2").put_value(32)
# Adding a sample value to "B3" cell
worksheet.cells.get("B3").put_value(50)
# Adding a sample value to "B4" cell
worksheet.cells.get("B4").put_value(40)
# Adding a sample value to "C1" cell as category data
worksheet.cells.get("C1").put_value("Q1")
# Adding a sample value to "C2" cell as category data
worksheet.cells.get("C2").put_value("Q2")
# Adding a sample value to "C3" cell as category data
worksheet.cells.get("C3").put_value("Y1")
# Adding a sample value to "C4" cell as category data
worksheet.cells.get("C4").put_value("Y2")
# Adding a chart to the worksheet
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 15, 5)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
seriesIndex = chart.n_series.add("A1:B4", True)
# Setting the data source for the category data of NSeries
chart.n_series.category_data = "C1:C4"
# Filling the area of the 2nd NSeries with a gradient
chart.n_series[seriesIndex].area.fill_format.set_one_color_gradient(Color.lime, 1, GradientStyleType.HORIZONTAL, 1)
```
### See Also
* module [`aspose.cells.drawing`](..)
