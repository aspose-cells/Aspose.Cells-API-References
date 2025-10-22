##ErrorBar class
## ErrorBar class
Represents error bar of data series.
**Inheritance:** [`ErrorBar`](/cells/python-net/aspose.cells.charts/errorbar) →
[`Line`](/cells/python-net/aspose.cells.drawing/line)
The ErrorBar type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [compound_type](/cells/python-net/aspose.cells.charts/errorbar/compound_type) | Specifies the compound line type |
| [dash_type](/cells/python-net/aspose.cells.charts/errorbar/dash_type) | Specifies the dash line type |
| [cap_type](/cells/python-net/aspose.cells.charts/errorbar/cap_type) | Specifies the ending caps. |
| [join_type](/cells/python-net/aspose.cells.charts/errorbar/join_type) | Specifies the joining caps. |
| [begin_type](/cells/python-net/aspose.cells.charts/errorbar/begin_type) | Specifies an arrowhead for the begin of a line. |
| [end_type](/cells/python-net/aspose.cells.charts/errorbar/end_type) | Specifies an arrowhead for the end of a line. |
| [begin_arrow_length](/cells/python-net/aspose.cells.charts/errorbar/begin_arrow_length) | Specifies the length of the arrowhead for the begin of a line. |
| [end_arrow_length](/cells/python-net/aspose.cells.charts/errorbar/end_arrow_length) | Specifies the length of the arrowhead for the end of a line. |
| [begin_arrow_width](/cells/python-net/aspose.cells.charts/errorbar/begin_arrow_width) | Specifies the width of the arrowhead for the begin of a line. |
| [end_arrow_width](/cells/python-net/aspose.cells.charts/errorbar/end_arrow_width) | Specifies the width of the arrowhead for the end of a line. |
| [theme_color](/cells/python-net/aspose.cells.charts/errorbar/theme_color) | Gets and sets the theme color. |
| [color](/cells/python-net/aspose.cells.charts/errorbar/color) | Represents the Color of the line. |
| [transparency](/cells/python-net/aspose.cells.charts/errorbar/transparency) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [style](/cells/python-net/aspose.cells.charts/errorbar/style) | Represents the style of the line. |
| [weight](/cells/python-net/aspose.cells.charts/errorbar/weight) | Gets or sets the [`WeightType`](/cells/python-net/aspose.cells.drawing/weighttype) of the line. |
| [weight_pt](/cells/python-net/aspose.cells.charts/errorbar/weight_pt) | Gets or sets the weight of the line in unit of points. |
| [weight_px](/cells/python-net/aspose.cells.charts/errorbar/weight_px) | Gets or sets the weight of the line in unit of pixels. |
| [formatting_type](/cells/python-net/aspose.cells.charts/errorbar/formatting_type) | Gets or sets format type. |
| [is_automatic_color](/cells/python-net/aspose.cells.charts/errorbar/is_automatic_color) | Indicates whether the color of line is automatic assigned. |
| [is_visible](/cells/python-net/aspose.cells.charts/errorbar/is_visible) | Represents whether the line is visible. |
| [is_auto](/cells/python-net/aspose.cells.charts/errorbar/is_auto) | Indicates whether this line style is auto assigned. |
| [gradient_fill](/cells/python-net/aspose.cells.charts/errorbar/gradient_fill) | Represents gradient fill. |
| [type](/cells/python-net/aspose.cells.charts/errorbar/type) | Represents error bar amount type. |
| [display_type](/cells/python-net/aspose.cells.charts/errorbar/display_type) | Represents the display type of error bar. |
| [amount](/cells/python-net/aspose.cells.charts/errorbar/amount) | Represents amount of error bar. |
| [show_marker_t_top](/cells/python-net/aspose.cells.charts/errorbar/show_marker_t_top) | Indicates if formatting error bars with a T-top. |
| [plus_value](/cells/python-net/aspose.cells.charts/errorbar/plus_value) | Represents positive error amount when error bar type is Custom. |
| [minus_value](/cells/python-net/aspose.cells.charts/errorbar/minus_value) | Represents negative error amount when error bar type is Custom. |
### Example
```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType, ErrorBarDisplayType, ErrorBarType
workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("a1").put_value(2)
cells.get("a2").put_value(5)
cells.get("a3").put_value(3)
cells.get("a4").put_value(6)
cells.get("b1").put_value(4)
cells.get("b2").put_value(3)
cells.get("b3").put_value(6)
cells.get("b4").put_value(7)
cells.get("C1").put_value("Q1")
cells.get("C2").put_value("Q2")
cells.get("C3").put_value("Y1")
cells.get("C4").put_value("Y2")
chartIndex = workbook.worksheets[0].charts.add(ChartType.COLUMN, 11, 0, 27, 10)
chart = workbook.worksheets[0].charts[chartIndex]
chart.n_series.add("A1:B4", True)
chart.n_series.category_data = "C1:C4"
for i in range(len(chart.n_series)):
aseries = chart.n_series[i]
aseries.y_error_bar.display_type = ErrorBarDisplayType.MINUS
aseries.y_error_bar.type = ErrorBarType.FIXED_VALUE
aseries.y_error_bar.amount = 5.0
```
### See Also
* module [`aspose.cells.charts`](..)
* class [`ErrorBar`](/cells/python-net/aspose.cells.charts/errorbar)
* class [`Line`](/cells/python-net/aspose.cells.drawing/line)
* class [`WeightType`](/cells/python-net/aspose.cells.drawing/weighttype)
