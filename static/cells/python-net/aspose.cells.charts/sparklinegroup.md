##SparklineGroup class
## SparklineGroup class
[`Sparkline`](/cells/python-net/aspose.cells.charts/sparkline) is organized into sparkline group. A SparklineGroup contains a variable number of sparkline items.
A sparkline group specifies the type, display settings and axis settings for the sparklines.
The SparklineGroup type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [preset_style](/cells/python-net/aspose.cells.charts/sparklinegroup/preset_style) | Gets and sets the preset style type of the sparkline group. |
| [sparkline_collection](/cells/python-net/aspose.cells.charts/sparklinegroup/sparkline_collection) | Gets the collection of [`Sparkline`](/cells/python-net/aspose.cells.charts/sparkline) object. |
| [sparklines](/cells/python-net/aspose.cells.charts/sparklinegroup/sparklines) | Gets the collection of [`Sparkline`](/cells/python-net/aspose.cells.charts/sparkline) object. |
| [type](/cells/python-net/aspose.cells.charts/sparklinegroup/type) | Indicates the sparkline type of the sparkline group. |
| [plot_empty_cells_type](/cells/python-net/aspose.cells.charts/sparklinegroup/plot_empty_cells_type) | Indicates how to plot empty cells. |
| [display_hidden](/cells/python-net/aspose.cells.charts/sparklinegroup/display_hidden) | Indicates whether to show data in hidden rows and columns. |
| [show_high_point](/cells/python-net/aspose.cells.charts/sparklinegroup/show_high_point) | Indicates whether to highlight the highest points of data in the sparkline group. |
| [high_point_color](/cells/python-net/aspose.cells.charts/sparklinegroup/high_point_color) | Gets and sets the color of the highest points of data in the sparkline group. |
| [show_low_point](/cells/python-net/aspose.cells.charts/sparklinegroup/show_low_point) | Indicates whether to highlight the lowest points of data in the sparkline group. |
| [low_point_color](/cells/python-net/aspose.cells.charts/sparklinegroup/low_point_color) | Gets and sets the color of the lowest points of data in the sparkline group. |
| [show_negative_points](/cells/python-net/aspose.cells.charts/sparklinegroup/show_negative_points) | Indicates whether to highlight the negative values on the sparkline group with a different color or marker. |
| [negative_points_color](/cells/python-net/aspose.cells.charts/sparklinegroup/negative_points_color) | Gets and sets the color of the negative values on the sparkline group. |
| [show_first_point](/cells/python-net/aspose.cells.charts/sparklinegroup/show_first_point) | Indicates whether to highlight the first point of data in the sparkline group. |
| [first_point_color](/cells/python-net/aspose.cells.charts/sparklinegroup/first_point_color) | Gets and sets the color of the first point of data in the sparkline group. |
| [show_last_point](/cells/python-net/aspose.cells.charts/sparklinegroup/show_last_point) | Indicates whether to highlight the last point of data in the sparkline group. |
| [last_point_color](/cells/python-net/aspose.cells.charts/sparklinegroup/last_point_color) | Gets and sets the color of the last point of data in the sparkline group. |
| [show_markers](/cells/python-net/aspose.cells.charts/sparklinegroup/show_markers) | Indicates whether to highlight each point in each line sparkline in the sparkline group. |
| [markers_color](/cells/python-net/aspose.cells.charts/sparklinegroup/markers_color) | Gets and sets the color of points in each line sparkline in the sparkline group. |
| [series_color](/cells/python-net/aspose.cells.charts/sparklinegroup/series_color) | Gets and sets the color of the sparklines in the sparkline group. |
| [plot_right_to_left](/cells/python-net/aspose.cells.charts/sparklinegroup/plot_right_to_left) | Indicates whether the plot data is right to left. |
| [line_weight](/cells/python-net/aspose.cells.charts/sparklinegroup/line_weight) | Gets and sets the line weight in each line sparkline in the sparkline group, in the unit of points. |
| [horizontal_axis_color](/cells/python-net/aspose.cells.charts/sparklinegroup/horizontal_axis_color) | Gets and sets the color of the horizontal axis in the sparkline group. |
| [show_horizontal_axis](/cells/python-net/aspose.cells.charts/sparklinegroup/show_horizontal_axis) | Indicates whether to show the sparkline horizontal axis.
| [horizontal_axis_date_range](/cells/python-net/aspose.cells.charts/sparklinegroup/horizontal_axis_date_range) | Represents the range that contains the date values for the sparkline data. |
| [vertical_axis_max_value_type](/cells/python-net/aspose.cells.charts/sparklinegroup/vertical_axis_max_value_type) | Represents the vertical axis maximum value type. |
| [vertical_axis_max_value](/cells/python-net/aspose.cells.charts/sparklinegroup/vertical_axis_max_value) | Gets and sets the custom maximum value for the vertical axis. |
| [vertical_axis_min_value_type](/cells/python-net/aspose.cells.charts/sparklinegroup/vertical_axis_min_value_type) | Represents the vertical axis minimum value type. |
| [vertical_axis_min_value](/cells/python-net/aspose.cells.charts/sparklinegroup/vertical_axis_min_value) | Gets and sets the custom minimum value for the vertical axis. |
### Methods
| Method | Description |
| :- | :- |
| [`reset_ranges(self, data_range, is_vertical, location_range)`](/cells/python-net/aspose.cells.charts/sparklinegroup/reset_ranges/#system.string-bool-aspose.cells.cellarea) | Resets the data range and location range of the sparkline group.
### Example
```python
from aspose.cells import CellArea, SaveFormat, Workbook
from aspose.cells.charts import SparklineType
from aspose.pydrawing import Color
book = Workbook()
sheet = book.worksheets[0]
sheet.cells.get("A1").put_value(5)
sheet.cells.get("B1").put_value(2)
sheet.cells.get("C1").put_value(1)
sheet.cells.get("D1").put_value(3)
#  Define the CellArea
ca = CellArea()
ca.start_column = 4
ca.end_column = 4
ca.start_row = 0
ca.end_row = 0
idx = sheet.sparkline_groups.add(SparklineType.LINE, "A1:D1", False, ca)
group = sheet.sparkline_groups[idx]
group.sparklines.add(sheet.name + "!A1:D1", 0, 4)
#  Create CellsColor
clr = book.create_cells_color()
clr.color = Color.orange
group.series_color = clr
#  set the high points are colored green and the low points are colored red
group.show_high_point = True
group.show_low_point = True
group.high_point_color.color = Color.green
group.low_point_color.color = Color.red
#  set line weight
group.line_weight = 1.0
book.save("output.xlsx", SaveFormat.XLSX)
```
### See Also
* module [`aspose.cells.charts`](..)
* class [`Sparkline`](/cells/python-net/aspose.cells.charts/sparkline)
