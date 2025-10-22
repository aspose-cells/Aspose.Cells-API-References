##Axis class
## Axis class
Encapsulates the object that represents an axis of chart.
The Axis type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [area](/cells/python-net/aspose.cells.charts/axis/area) | Gets the [`Axis.area`](/cells/python-net/aspose.cells.charts/axis#area). |
| [is_automatic_min_value](/cells/python-net/aspose.cells.charts/axis/is_automatic_min_value) | Indicates whether the min value is automatically assigned. |
| [min_value](/cells/python-net/aspose.cells.charts/axis/min_value) | Represents the minimum value on the value axis. |
| [is_automatic_max_value](/cells/python-net/aspose.cells.charts/axis/is_automatic_max_value) | Indicates whether the max value is automatically assigned. |
| [max_value](/cells/python-net/aspose.cells.charts/axis/max_value) | Represents the maximum value on the value axis. |
| [is_automatic_major_unit](/cells/python-net/aspose.cells.charts/axis/is_automatic_major_unit) | Indicates whether the major unit of the axis is automatically assigned. |
| [major_unit](/cells/python-net/aspose.cells.charts/axis/major_unit) | Represents the major units for the axis. |
| [is_automatic_minor_unit](/cells/python-net/aspose.cells.charts/axis/is_automatic_minor_unit) | Indicates whether the minor unit of the axis is automatically assigned. |
| [minor_unit](/cells/python-net/aspose.cells.charts/axis/minor_unit) | Represents the minor units for the axis. |
| [axis_line](/cells/python-net/aspose.cells.charts/axis/axis_line) | Gets the appearance of an Axis. |
| [major_tick_mark](/cells/python-net/aspose.cells.charts/axis/major_tick_mark) | Represents the type of major tick mark for the specified axis. |
| [minor_tick_mark](/cells/python-net/aspose.cells.charts/axis/minor_tick_mark) | Represents the type of minor tick mark for the specified axis. |
| [tick_label_position](/cells/python-net/aspose.cells.charts/axis/tick_label_position) | Represents the position of tick-mark labels on the specified axis. |
| [cross_at](/cells/python-net/aspose.cells.charts/axis/cross_at) | Represents the point on the value axis where the category axis crosses it. |
| [cross_type](/cells/python-net/aspose.cells.charts/axis/cross_type) | Represents the [`Axis.cross_type`](/cells/python-net/aspose.cells.charts/axis#cross_type) on the specified axis where the other axis crosses. |
| [log_base](/cells/python-net/aspose.cells.charts/axis/log_base) | Represents the logarithmic base. Default value is 10.Only applies for Excel2007. |
| [is_logarithmic](/cells/python-net/aspose.cells.charts/axis/is_logarithmic) | Represents if the value axis scale type is logarithmic or not. |
| [is_plot_order_reversed](/cells/python-net/aspose.cells.charts/axis/is_plot_order_reversed) | Represents if Microsoft Excel plots data points from last to first. |
| [axis_between_categories](/cells/python-net/aspose.cells.charts/axis/axis_between_categories) | Represents if the value axis crosses the category axis between categories. |
| [tick_labels](/cells/python-net/aspose.cells.charts/axis/tick_labels) | Returns a [`Axis.tick_labels`](/cells/python-net/aspose.cells.charts/axis#tick_labels) object that represents the tick-mark labels for the specified axis. |
| [tick_label_spacing](/cells/python-net/aspose.cells.charts/axis/tick_label_spacing) | Represents the number of categories or series between tick-mark labels. Applies only to category and series axes. |
| [is_auto_tick_label_spacing](/cells/python-net/aspose.cells.charts/axis/is_auto_tick_label_spacing) | Indicates whether the spacing of tick label is automatic |
| [tick_mark_spacing](/cells/python-net/aspose.cells.charts/axis/tick_mark_spacing) | Returns or sets the number of categories or series between tick marks. Applies only to category and series axes. |
| [display_unit](/cells/python-net/aspose.cells.charts/axis/display_unit) | Represents the unit label for the specified axis. |
| [cust_unit](/cells/python-net/aspose.cells.charts/axis/cust_unit) | Specifies a custom value for the display unit. |
| [custom_unit](/cells/python-net/aspose.cells.charts/axis/custom_unit) | Specifies a custom value for the display unit. |
| [custom_display_unit](/cells/python-net/aspose.cells.charts/axis/custom_display_unit) | Specifies a custom value for the display unit. |
| [display_unit_label](/cells/python-net/aspose.cells.charts/axis/display_unit_label) | Represents a unit label on an axis in the specified chart.
| [is_display_unit_label_shown](/cells/python-net/aspose.cells.charts/axis/is_display_unit_label_shown) | Represents if the display unit label is shown on the specified axis. |
| [title](/cells/python-net/aspose.cells.charts/axis/title) | Gets the axis' title. |
| [category_type](/cells/python-net/aspose.cells.charts/axis/category_type) | Represents the category axis type. |
| [base_unit_scale](/cells/python-net/aspose.cells.charts/axis/base_unit_scale) | Represents the base unit scale for the category axis. |
| [major_unit_scale](/cells/python-net/aspose.cells.charts/axis/major_unit_scale) | Represents the major unit scale for the category axis. |
| [minor_unit_scale](/cells/python-net/aspose.cells.charts/axis/minor_unit_scale) | Represents the major unit scale for the category axis. |
| [is_visible](/cells/python-net/aspose.cells.charts/axis/is_visible) | Represents if the axis is visible. |
| [major_grid_lines](/cells/python-net/aspose.cells.charts/axis/major_grid_lines) | Represents major gridlines on a chart axis. |
| [minor_grid_lines](/cells/python-net/aspose.cells.charts/axis/minor_grid_lines) | Represents minor gridlines on a chart axis. |
| [has_multi_level_labels](/cells/python-net/aspose.cells.charts/axis/has_multi_level_labels) | Indicates whether the labels shall be shown as multi level. |
| [axis_labels](/cells/python-net/aspose.cells.charts/axis/axis_labels) | Gets the labels of the axis after call Chart.Calculate() method. |
| [bins](/cells/python-net/aspose.cells.charts/axis/bins) | Represents bins on a chart(Histogram/Pareto) axis |
### Methods
| Method | Description |
| :- | :- |
| [`get_axis_texts(self)`](/cells/python-net/aspose.cells.charts/axis/get_axis_texts/#) | Gets the labels of the axis after call Chart.Calculate() method. |
### Example
From the following codes , you can learn how to set unit, maximum and minimum value  of Axis.
```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType, CrossType
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
# Adding a sample value to "B1" cell
worksheet.cells.get("B1").put_value(4)
# Adding a sample value to "B2" cell
worksheet.cells.get("B2").put_value(20)
# Adding a sample value to "B3" cell
worksheet.cells.get("B3").put_value(50)
# Adding a chart to the worksheet
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 25, 5)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.n_series.add("A1:B3", True)
# Set the max value of value axis
chart.value_axis.max_value = 200
# Set the min value of value axis
chart.value_axis.min_value = 0
# Set the major unit
chart.value_axis.major_unit = 25.0
# Category(X) axis crosses at the maxinum value.
chart.value_axis.cross_type = CrossType.MAXIMUM
# Set he number of categories or series between tick-mark labels.
chart.category_axis.tick_label_spacing = 2
# do your business
# Saving the Excel file
workbook.save("book1.xlsx")
```
### See Also
* module [`aspose.cells.charts`](..)
