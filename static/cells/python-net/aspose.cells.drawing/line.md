##Line class
## Line class
Encapsulates the object that represents the line format.
The Line type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [compound_type](/cells/python-net/aspose.cells.drawing/line/compound_type) | Specifies the compound line type |
| [dash_type](/cells/python-net/aspose.cells.drawing/line/dash_type) | Specifies the dash line type |
| [cap_type](/cells/python-net/aspose.cells.drawing/line/cap_type) | Specifies the ending caps. |
| [join_type](/cells/python-net/aspose.cells.drawing/line/join_type) | Specifies the joining caps. |
| [begin_type](/cells/python-net/aspose.cells.drawing/line/begin_type) | Specifies an arrowhead for the begin of a line. |
| [end_type](/cells/python-net/aspose.cells.drawing/line/end_type) | Specifies an arrowhead for the end of a line. |
| [begin_arrow_length](/cells/python-net/aspose.cells.drawing/line/begin_arrow_length) | Specifies the length of the arrowhead for the begin of a line. |
| [end_arrow_length](/cells/python-net/aspose.cells.drawing/line/end_arrow_length) | Specifies the length of the arrowhead for the end of a line. |
| [begin_arrow_width](/cells/python-net/aspose.cells.drawing/line/begin_arrow_width) | Specifies the width of the arrowhead for the begin of a line. |
| [end_arrow_width](/cells/python-net/aspose.cells.drawing/line/end_arrow_width) | Specifies the width of the arrowhead for the end of a line. |
| [theme_color](/cells/python-net/aspose.cells.drawing/line/theme_color) | Gets and sets the theme color. |
| [color](/cells/python-net/aspose.cells.drawing/line/color) | Represents the Color of the line. |
| [transparency](/cells/python-net/aspose.cells.drawing/line/transparency) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [style](/cells/python-net/aspose.cells.drawing/line/style) | Represents the style of the line. |
| [weight](/cells/python-net/aspose.cells.drawing/line/weight) | Gets or sets the [`WeightType`](/cells/python-net/aspose.cells.drawing/weighttype) of the line. |
| [weight_pt](/cells/python-net/aspose.cells.drawing/line/weight_pt) | Gets or sets the weight of the line in unit of points. |
| [weight_px](/cells/python-net/aspose.cells.drawing/line/weight_px) | Gets or sets the weight of the line in unit of pixels. |
| [formatting_type](/cells/python-net/aspose.cells.drawing/line/formatting_type) | Gets or sets format type. |
| [is_automatic_color](/cells/python-net/aspose.cells.drawing/line/is_automatic_color) | Indicates whether the color of line is automatic assigned. |
| [is_visible](/cells/python-net/aspose.cells.drawing/line/is_visible) | Represents whether the line is visible. |
| [is_auto](/cells/python-net/aspose.cells.drawing/line/is_auto) | Indicates whether this line style is auto assigned. |
| [gradient_fill](/cells/python-net/aspose.cells.drawing/line/gradient_fill) | Represents gradient fill. |
### Example
```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartMarkerType, ChartType
from aspose.cells.drawing import LineType, WeightType
from aspose.pydrawing import Color
workbook = Workbook()
sheet = workbook.worksheets[0]
cells = sheet.cells
cells.get(0, 1).put_value("Income")
cells.get(1, 0).put_value("Company A")
cells.get(2, 0).put_value("Company B")
cells.get(3, 0).put_value("Company C")
cells.get(1, 1).put_value(10000)
cells.get(2, 1).put_value(20000)
cells.get(3, 1).put_value(30000)
chartIndex = sheet.charts.add(ChartType.LINE, 9, 9, 21, 15)
chart = sheet.charts[chartIndex]
# Add series
chart.n_series.add("A2:B4", True)
# Set category data
chart.n_series.category_data = "=Sheet1!$A$2:$A$4"
# Applying a dotted line style on the lines of an NSeries
chart.n_series[0].border.style = LineType.DOT
chart.n_series[0].border.color = Color.red
# Applying a triangular marker style on the data markers of an NSeries
chart.n_series[0].marker.marker_style = ChartMarkerType.TRIANGLE
# Setting the weight of all lines in an NSeries to medium
chart.n_series[0].border.weight = WeightType.MEDIUM_LINE
```
### See Also
* module [`aspose.cells.drawing`](..)
* class [`WeightType`](/cells/python-net/aspose.cells.drawing/weighttype)
