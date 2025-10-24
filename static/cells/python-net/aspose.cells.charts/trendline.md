##Trendline class
## Trendline class
Represents a trendline in a chart.
**Inheritance:** [`Trendline`](/cells/python-net/aspose.cells.charts/trendline) →
[`Line`](/cells/python-net/aspose.cells.drawing/line)
The Trendline type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [compound_type](/cells/python-net/aspose.cells.charts/trendline/compound_type) | Specifies the compound line type |
| [dash_type](/cells/python-net/aspose.cells.charts/trendline/dash_type) | Specifies the dash line type |
| [cap_type](/cells/python-net/aspose.cells.charts/trendline/cap_type) | Specifies the ending caps. |
| [join_type](/cells/python-net/aspose.cells.charts/trendline/join_type) | Specifies the joining caps. |
| [begin_type](/cells/python-net/aspose.cells.charts/trendline/begin_type) | Specifies an arrowhead for the begin of a line. |
| [end_type](/cells/python-net/aspose.cells.charts/trendline/end_type) | Specifies an arrowhead for the end of a line. |
| [begin_arrow_length](/cells/python-net/aspose.cells.charts/trendline/begin_arrow_length) | Specifies the length of the arrowhead for the begin of a line. |
| [end_arrow_length](/cells/python-net/aspose.cells.charts/trendline/end_arrow_length) | Specifies the length of the arrowhead for the end of a line. |
| [begin_arrow_width](/cells/python-net/aspose.cells.charts/trendline/begin_arrow_width) | Specifies the width of the arrowhead for the begin of a line. |
| [end_arrow_width](/cells/python-net/aspose.cells.charts/trendline/end_arrow_width) | Specifies the width of the arrowhead for the end of a line. |
| [theme_color](/cells/python-net/aspose.cells.charts/trendline/theme_color) | Gets and sets the theme color. |
| [color](/cells/python-net/aspose.cells.charts/trendline/color) | Represents the Color of the line. |
| [transparency](/cells/python-net/aspose.cells.charts/trendline/transparency) | Returns or sets the degree of transparency of the line as a value from 0.0 (opaque) through 1.0 (clear). |
| [style](/cells/python-net/aspose.cells.charts/trendline/style) | Represents the style of the line. |
| [weight](/cells/python-net/aspose.cells.charts/trendline/weight) | Gets or sets the [`WeightType`](/cells/python-net/aspose.cells.drawing/weighttype) of the line. |
| [weight_pt](/cells/python-net/aspose.cells.charts/trendline/weight_pt) | Gets or sets the weight of the line in unit of points. |
| [weight_px](/cells/python-net/aspose.cells.charts/trendline/weight_px) | Gets or sets the weight of the line in unit of pixels. |
| [formatting_type](/cells/python-net/aspose.cells.charts/trendline/formatting_type) | Gets or sets format type. |
| [is_automatic_color](/cells/python-net/aspose.cells.charts/trendline/is_automatic_color) | Indicates whether the color of line is automatic assigned. |
| [is_visible](/cells/python-net/aspose.cells.charts/trendline/is_visible) | Represents whether the line is visible. |
| [is_auto](/cells/python-net/aspose.cells.charts/trendline/is_auto) | Indicates whether this line style is auto assigned. |
| [gradient_fill](/cells/python-net/aspose.cells.charts/trendline/gradient_fill) | Represents gradient fill. |
| [is_name_auto](/cells/python-net/aspose.cells.charts/trendline/is_name_auto) | Returns if Microsoft Excel automatically determines the name of the trendline. |
| [type](/cells/python-net/aspose.cells.charts/trendline/type) | Returns the trendline type. |
| [name](/cells/python-net/aspose.cells.charts/trendline/name) | Returns the name of the trendline. |
| [order](/cells/python-net/aspose.cells.charts/trendline/order) | Returns or sets the trendline order (an integer greater than 1) when the trendline type is Polynomial.
| [period](/cells/python-net/aspose.cells.charts/trendline/period) | Returns or sets the period for the moving-average trendline. |
| [forward](/cells/python-net/aspose.cells.charts/trendline/forward) | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends forward.
| [backward](/cells/python-net/aspose.cells.charts/trendline/backward) | Returns or sets the number of periods (or units on a scatter chart) that the trendline extends backward.
| [display_equation](/cells/python-net/aspose.cells.charts/trendline/display_equation) | Represents if the equation for the trendline is displayed on the chart (in the same data label as the R-squared value). Setting this property to True automatically turns on data labels. |
| [display_r_squared](/cells/python-net/aspose.cells.charts/trendline/display_r_squared) | Represents if the R-squared value of the trendline is displayed on the chart (in the same data label as the equation). Setting this property to True automatically turns on data labels. |
| [intercept](/cells/python-net/aspose.cells.charts/trendline/intercept) | Returns or sets the point where the trendline crosses the value axis. |
| [data_labels](/cells/python-net/aspose.cells.charts/trendline/data_labels) | Represents the DataLabels object for the specified series. |
| [legend_entry](/cells/python-net/aspose.cells.charts/trendline/legend_entry) | Gets the legend entry according to this trendline |
### Example
```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType, TrendlineType
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
chart.n_series.add("A1:B4", True)
# Setting the data source for the category data of NSeries
chart.n_series.category_data = "C1:C4"
# adding a linear trendline
index = chart.n_series[0].trend_lines.add(TrendlineType.LINEAR)
trendline = chart.n_series[0].trend_lines[index]
# Setting the custom name of the trendline.
trendline.name = "Linear"
# Displaying the equation on chart
trendline.display_equation = True
# Displaying the R-Squared value on chart
trendline.display_r_squared = True
# Saving the Excel file
workbook.save("book1.xls")
```
### See Also
* module [`aspose.cells.charts`](..)
* class [`Line`](/cells/python-net/aspose.cells.drawing/line)
* class [`Trendline`](/cells/python-net/aspose.cells.charts/trendline)
* class [`WeightType`](/cells/python-net/aspose.cells.drawing/weighttype)
