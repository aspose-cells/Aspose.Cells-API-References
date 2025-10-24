##ChartPoint class
## ChartPoint class
Represents a single point in a series in a chart.
The ChartPoint type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [explosion](/cells/python-net/aspose.cells.charts/chartpoint/explosion) | The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter. |
| [shadow](/cells/python-net/aspose.cells.charts/chartpoint/shadow) | True if the chartpoint has a shadow. |
| [border](/cells/python-net/aspose.cells.charts/chartpoint/border) | Gets the [`Line`](/cells/python-net/aspose.cells.drawing/line). |
| [area](/cells/python-net/aspose.cells.charts/chartpoint/area) | Gets the [`ChartPoint.area`](/cells/python-net/aspose.cells.charts/chartpoint#area). |
| [marker](/cells/python-net/aspose.cells.charts/chartpoint/marker) | Gets the [`ChartPoint.marker`](/cells/python-net/aspose.cells.charts/chartpoint#marker). |
| [data_labels](/cells/python-net/aspose.cells.charts/chartpoint/data_labels) | Returns a [`ChartPoint.data_labels`](/cells/python-net/aspose.cells.charts/chartpoint#data_labels) object that represents the data label associated with this chart point. |
| [y_value](/cells/python-net/aspose.cells.charts/chartpoint/y_value) | Gets or sets the Y value of the chart point. |
| [y_value_type](/cells/python-net/aspose.cells.charts/chartpoint/y_value_type) | Gets Y value type of the chart point. |
| [x_value](/cells/python-net/aspose.cells.charts/chartpoint/x_value) | Gets or sets the X value of the chart point. |
| [x_value_type](/cells/python-net/aspose.cells.charts/chartpoint/x_value_type) | Gets X value type of the chart point. |
| [shape_properties](/cells/python-net/aspose.cells.charts/chartpoint/shape_properties) | Gets the [`ShapePropertyCollection`](/cells/python-net/aspose.cells.drawing/shapepropertycollection) object that holds the visual shape properties of the ChartPoint. |
| [is_in_secondary_plot](/cells/python-net/aspose.cells.charts/chartpoint/is_in_secondary_plot) | Gets or sets a value indicates whether this data points is in the second pie or bar
| [shape_x](/cells/python-net/aspose.cells.charts/chartpoint/shape_x) | Gets the x coordinate of the upper left corner in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [shape_y](/cells/python-net/aspose.cells.charts/chartpoint/shape_y) | Gets the y coordinate of the upper left corner in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [shape_width](/cells/python-net/aspose.cells.charts/chartpoint/shape_width) | Gets the width in units of 1/4000 of chart's width after calls Chart.Calculate() method. |
| [shape_height](/cells/python-net/aspose.cells.charts/chartpoint/shape_height) | Gets the height in units of 1/4000 of chart's height after calls Chart.Calculate() method. |
| [shape_x_px](/cells/python-net/aspose.cells.charts/chartpoint/shape_x_px) | Gets the x coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method. |
| [shape_y_px](/cells/python-net/aspose.cells.charts/chartpoint/shape_y_px) | Gets the y coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method. |
| [shape_width_px](/cells/python-net/aspose.cells.charts/chartpoint/shape_width_px) | Gets the width in units of pixels after calls Chart.Calculate() method. |
| [shape_height_px](/cells/python-net/aspose.cells.charts/chartpoint/shape_height_px) | Gets the height in units of pixels after calls Chart.Calculate() method. |
| [border_width_px](/cells/python-net/aspose.cells.charts/chartpoint/border_width_px) | Gets the width of border in units of pixels after calls Chart.Calculate() method. |
| [radius_px](/cells/python-net/aspose.cells.charts/chartpoint/radius_px) | Gets the radius of bubble, pie or doughnut in units of pixels after calls Chart.Calculate() method. |
| [doughnut_inner_radius](/cells/python-net/aspose.cells.charts/chartpoint/doughnut_inner_radius) | Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method.
| [inner_radius_px](/cells/python-net/aspose.cells.charts/chartpoint/inner_radius_px) | Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method.
| [start_angle](/cells/python-net/aspose.cells.charts/chartpoint/start_angle) | Gets the starting angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method.
| [end_angle](/cells/python-net/aspose.cells.charts/chartpoint/end_angle) | Gets the ending angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method.
| [arc_start_point_x_px](/cells/python-net/aspose.cells.charts/chartpoint/arc_start_point_x_px) | Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method.
| [arc_start_point_y_px](/cells/python-net/aspose.cells.charts/chartpoint/arc_start_point_y_px) | Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method.
| [arc_end_point_x_px](/cells/python-net/aspose.cells.charts/chartpoint/arc_end_point_x_px) | Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method.
| [arc_end_point_y_px](/cells/python-net/aspose.cells.charts/chartpoint/arc_end_point_y_px) | Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method.
| [inner_arc_start_point_x_px](/cells/python-net/aspose.cells.charts/chartpoint/inner_arc_start_point_x_px) | Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method.
| [inner_arc_start_point_y_px](/cells/python-net/aspose.cells.charts/chartpoint/inner_arc_start_point_y_px) | Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method.
| [inner_arc_end_point_x_px](/cells/python-net/aspose.cells.charts/chartpoint/inner_arc_end_point_x_px) | Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method.
| [inner_arc_end_point_y_px](/cells/python-net/aspose.cells.charts/chartpoint/inner_arc_end_point_y_px) | Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method.
### Methods
| Method | Description |
| :- | :- |
| [`get_top_point_count(self)`](/cells/python-net/aspose.cells.charts/chartpoint/get_top_point_count/#) | Gets the number of top points after calls Chart.Calculate() method. |
| [`get_top_point_x_px(self, index)`](/cells/python-net/aspose.cells.charts/chartpoint/get_top_point_x_px/#int) | Gets x-coordinate of the top point of shape after calls Chart.Calculate() method.
| [`get_top_point_y_px(self, index)`](/cells/python-net/aspose.cells.charts/chartpoint/get_top_point_y_px/#int) | Gets y-coordinate of the top point of shape after calls Chart.Calculate() method.
| [`get_bottom_point_count(self)`](/cells/python-net/aspose.cells.charts/chartpoint/get_bottom_point_count/#) | Gets the number of bottom points  after calls Chart.Calculate() method. |
| [`get_bottom_point_x_px(self, index)`](/cells/python-net/aspose.cells.charts/chartpoint/get_bottom_point_x_px/#int) | Gets x-coordinate of the bottom point of shape after calls Chart.Calculate() method.
| [`get_bottom_point_y_px(self, index)`](/cells/python-net/aspose.cells.charts/chartpoint/get_bottom_point_y_px/#int) | Gets y-coordinate of the bottom point of shape  after calls Chart.Calculate() method.
| [`get_on_category_axis_point_count(self)`](/cells/python-net/aspose.cells.charts/chartpoint/get_on_category_axis_point_count/#) | Gets the number of the points on category axis after calls Chart.Calculate() method. Only applies to area chart. |
| [`get_on_category_axis_point_x_px(self, index)`](/cells/python-net/aspose.cells.charts/chartpoint/get_on_category_axis_point_x_px/#int) | Gets x-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart. |
| [`get_on_category_axis_point_y_px(self, index)`](/cells/python-net/aspose.cells.charts/chartpoint/get_on_category_axis_point_y_px/#int) | Gets y-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart. |
### Example
```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType
from aspose.pydrawing import Color
# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Adding a sample value to "A1" cell
worksheet.cells.get("A1").put_value(50)
# Adding a sample value to "A2" cell
worksheet.cells.get("A2").put_value(100)
# Adding a sample value to "A3" cell
worksheet.cells.get("A3").put_value(150)
# Adding a sample value to "B1" cell
worksheet.cells.get("B1").put_value(60)
# Adding a sample value to "B2" cell
worksheet.cells.get("B2").put_value(32)
# Adding a sample value to "B3" cell
worksheet.cells.get("B3").put_value(50)
# Adding a chart to the worksheet
chartIndex = worksheet.charts.add(ChartType.PIE_EXPLODED, 5, 0, 25, 10)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.n_series.add("A1:B3", True)
# Show Data Labels
chart.n_series[0].data_labels.show_value = True
for i in range(chart.n_series[0].points.count):
# Get Data Point
point = chart.n_series[0].points[i]
# Set Pir Explosion
point.explosion = 15
# Set Border Color
point.border.color = Color.red
# Saving the Excel file
workbook.save("book1.xls")
```
### See Also
* module [`aspose.cells.charts`](..)
* class [`Line`](/cells/python-net/aspose.cells.drawing/line)
* class [`ShapePropertyCollection`](/cells/python-net/aspose.cells.drawing/shapepropertycollection)
