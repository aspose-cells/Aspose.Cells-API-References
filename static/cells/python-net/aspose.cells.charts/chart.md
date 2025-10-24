##Chart class
## Chart class
Encapsulates the object that represents a single Excel chart.
The Chart type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [style](/cells/python-net/aspose.cells.charts/chart/style) | Gets and sets the builtin style. |
| [chart_object](/cells/python-net/aspose.cells.charts/chart/chart_object) | Represents the chartShape; |
| [hide_pivot_field_buttons](/cells/python-net/aspose.cells.charts/chart/hide_pivot_field_buttons) | Indicates whether hide the pivot chart field buttons only when the chart is PivotChart. |
| [pivot_options](/cells/python-net/aspose.cells.charts/chart/pivot_options) | Specifies the pivot controls that appear on the chart |
| [pivot_source](/cells/python-net/aspose.cells.charts/chart/pivot_source) | The source is the data of the pivotTable.
| [plot_by](/cells/python-net/aspose.cells.charts/chart/plot_by) | Gets and sets whether plot by row or column. |
| [plot_empty_cells_type](/cells/python-net/aspose.cells.charts/chart/plot_empty_cells_type) | Gets and sets  how to plot the empty cells. |
| [plot_visible_cells](/cells/python-net/aspose.cells.charts/chart/plot_visible_cells) | Indicates whether only plot visible cells. |
| [plot_visible_cells_only](/cells/python-net/aspose.cells.charts/chart/plot_visible_cells_only) | Indicates whether plot visible cells only. |
| [display_na_as_blank](/cells/python-net/aspose.cells.charts/chart/display_na_as_blank) | Indicates whether displaying #N/A as blank value. |
| [name](/cells/python-net/aspose.cells.charts/chart/name) | Gets and sets the name of the chart. |
| [size_with_window](/cells/python-net/aspose.cells.charts/chart/size_with_window) | True if Microsoft Excel resizes the chart to match the size of the chart sheet window. |
| [worksheet](/cells/python-net/aspose.cells.charts/chart/worksheet) | Gets the worksheet which contains this chart. |
| [shapes](/cells/python-net/aspose.cells.charts/chart/shapes) | Returns all drawing shapes in this chart. |
| [print_size](/cells/python-net/aspose.cells.charts/chart/print_size) | Gets and sets the printed chart size. |
| [type](/cells/python-net/aspose.cells.charts/chart/type) | Gets or sets a chart's type. |
| [n_series](/cells/python-net/aspose.cells.charts/chart/n_series) | Gets a [`SeriesCollection`](/cells/python-net/aspose.cells.charts/seriescollection) collection representing the data series in the chart. |
| [filtered_n_series](/cells/python-net/aspose.cells.charts/chart/filtered_n_series) | Gets a [`SeriesCollection`](/cells/python-net/aspose.cells.charts/seriescollection) collection representing the data series that are filtered in the chart. |
| [title](/cells/python-net/aspose.cells.charts/chart/title) | Gets the chart's title. |
| [sub_title](/cells/python-net/aspose.cells.charts/chart/sub_title) | Gets the chart's sub-title.
| [plot_area](/cells/python-net/aspose.cells.charts/chart/plot_area) | Gets the chart's plot area which includes axis tick labels. |
| [chart_area](/cells/python-net/aspose.cells.charts/chart/chart_area) | Gets the chart area in the worksheet. |
| [category_axis](/cells/python-net/aspose.cells.charts/chart/category_axis) | Gets the chart's X axis. |
| [value_axis](/cells/python-net/aspose.cells.charts/chart/value_axis) | Gets the chart's Y axis. |
| [second_value_axis](/cells/python-net/aspose.cells.charts/chart/second_value_axis) | Gets the chart's second Y axis. |
| [second_category_axis](/cells/python-net/aspose.cells.charts/chart/second_category_axis) | Gets the chart's second X axis. |
| [series_axis](/cells/python-net/aspose.cells.charts/chart/series_axis) | Gets the chart's series axis. |
| [legend](/cells/python-net/aspose.cells.charts/chart/legend) | Gets the chart legend. |
| [chart_data_table](/cells/python-net/aspose.cells.charts/chart/chart_data_table) | Represents the chart data table. |
| [show_legend](/cells/python-net/aspose.cells.charts/chart/show_legend) | Gets or sets a value indicating whether the chart legend will be displayed. Default is true. |
| [is_rectangular_cornered](/cells/python-net/aspose.cells.charts/chart/is_rectangular_cornered) | Gets or sets a value indicating whether the chart area is rectangular cornered.
| [show_data_table](/cells/python-net/aspose.cells.charts/chart/show_data_table) | Gets or sets a value indicating whether the chart displays a data table. |
| [first_slice_angle](/cells/python-net/aspose.cells.charts/chart/first_slice_angle) | Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical).
| [gap_width](/cells/python-net/aspose.cells.charts/chart/gap_width) | Returns or sets the space between bar or column clusters, as a percentage of the bar or column width.
| [gap_depth](/cells/python-net/aspose.cells.charts/chart/gap_depth) | Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width.
| [floor](/cells/python-net/aspose.cells.charts/chart/floor) | Returns a [`Chart.floor`](/cells/python-net/aspose.cells.charts/chart#floor) object that represents the walls of a 3-D chart. |
| [walls](/cells/python-net/aspose.cells.charts/chart/walls) | Returns a [`Chart.walls`](/cells/python-net/aspose.cells.charts/chart#walls) object that represents the walls of a 3-D chart. |
| [back_wall](/cells/python-net/aspose.cells.charts/chart/back_wall) | Returns a [`Chart.walls`](/cells/python-net/aspose.cells.charts/chart#walls) object that represents the back wall of a 3-D chart. |
| [side_wall](/cells/python-net/aspose.cells.charts/chart/side_wall) | Returns a [`Chart.walls`](/cells/python-net/aspose.cells.charts/chart#walls) object that represents the side wall of a 3-D chart. |
| [walls_and_gridlines_2d](/cells/python-net/aspose.cells.charts/chart/walls_and_gridlines_2d) | True if gridlines are drawn two-dimensionally on a 3-D chart. |
| [rotation_angle](/cells/python-net/aspose.cells.charts/chart/rotation_angle) | Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees). |
| [elevation](/cells/python-net/aspose.cells.charts/chart/elevation) | Represents the elevation of the 3-D chart view, in degrees. |
| [right_angle_axes](/cells/python-net/aspose.cells.charts/chart/right_angle_axes) | True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie Charts). |
| [auto_scaling](/cells/python-net/aspose.cells.charts/chart/auto_scaling) | True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart.
| [height_percent](/cells/python-net/aspose.cells.charts/chart/height_percent) | Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent). |
| [perspective](/cells/python-net/aspose.cells.charts/chart/perspective) | Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100.
| [is_3d](/cells/python-net/aspose.cells.charts/chart/is_3d) | Indicates whether the chart is a 3d chart. |
| [depth_percent](/cells/python-net/aspose.cells.charts/chart/depth_percent) | Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent). |
| [actual_chart_size](/cells/python-net/aspose.cells.charts/chart/actual_chart_size) | Gets actual size of chart in unit of pixels. |
| [placement](/cells/python-net/aspose.cells.charts/chart/placement) | Represents the way the chart is attached to the cells below it. |
| [page_setup](/cells/python-net/aspose.cells.charts/chart/page_setup) | Represents the page setup description in this chart. |
| [line](/cells/python-net/aspose.cells.charts/chart/line) | Gets the line. |
### Methods
| Method | Description |
| :- | :- |
| [`calculate(self)`](/cells/python-net/aspose.cells.charts/chart/calculate/#) | Calculates the custom position of plot area, axes if the position of them are auto assigned. |
| [`calculate(self, calculate_options)`](/cells/python-net/aspose.cells.charts/chart/calculate/#aspose.cells.charts.chartcalculateoptions) | Calculates the custom position of plot area, axes if the position of them are auto assigned, with Chart Calculate Options. |
| [`to_image(self, image_file)`](/cells/python-net/aspose.cells.charts/chart/to_image/#system.string) | Creates the chart image and saves it to a file.
| [`to_image(self, image_file, image_type)`](/cells/python-net/aspose.cells.charts/chart/to_image/#system.string-aspose.cells.drawing.imagetype) | Creates the chart image and saves it to a file in the specified image type. |
| [`to_image(self, image_file, jpeg_quality)`](/cells/python-net/aspose.cells.charts/chart/to_image/#system.string-int) | Creates the chart image and saves it to a file in the Jpeg format. |
| [`to_image(self, stream, jpeg_quality)`](/cells/python-net/aspose.cells.charts/chart/to_image/#io.rawiobase-int) | Creates the chart image and saves it to a stream in the Jpeg format. |
| [`to_image(self, stream, image_type)`](/cells/python-net/aspose.cells.charts/chart/to_image/#io.rawiobase-aspose.cells.drawing.imagetype) | Creates the chart image and saves it to a stream in the specified format. |
| [`to_image(self, image_file, options)`](/cells/python-net/aspose.cells.charts/chart/to_image/#system.string-aspose.cells.rendering.imageorprintoptions) | Creates the chart image and saves it to a file.
| [`to_image(self, stream, options)`](/cells/python-net/aspose.cells.charts/chart/to_image/#io.rawiobase-aspose.cells.rendering.imageorprintoptions) | Creates the chart image and saves it to a stream in the specified format. |
| [`to_pdf(self, file_name)`](/cells/python-net/aspose.cells.charts/chart/to_pdf/#system.string) | Saves the chart to a pdf file. |
| [`to_pdf(self, file_name, desired_page_width, desired_page_height, h_alignment_type, v_alignment_type)`](/cells/python-net/aspose.cells.charts/chart/to_pdf/#system.string-float-float-aspose.cells.pagelayoutalignmenttype-aspose.cells.pagelayoutalignmenttype) | Saves the chart to a pdf file. |
| [`to_pdf(self, stream)`](/cells/python-net/aspose.cells.charts/chart/to_pdf/#io.rawiobase) | Creates the chart pdf and saves it to a stream. |
| [`to_pdf(self, stream, desired_page_width, desired_page_height, h_alignment_type, v_alignment_type)`](/cells/python-net/aspose.cells.charts/chart/to_pdf/#io.rawiobase-float-float-aspose.cells.pagelayoutalignmenttype-aspose.cells.pagelayoutalignmenttype) | Creates the chart pdf and saves it to a stream. |
| [`is_refered_by_chart(self, row_index, column_index)`](/cells/python-net/aspose.cells.charts/chart/is_refered_by_chart/#int-int) | Returns whether the cell refered by the chart. |
| [`is_cell_refered_by_chart(self, sheet_index, row_index, column_index)`](/cells/python-net/aspose.cells.charts/chart/is_cell_refered_by_chart/#int-int-int) | Returns whether the cell refered by the chart. |
| [`is_chart_data_changed(self)`](/cells/python-net/aspose.cells.charts/chart/is_chart_data_changed/#) | Detects if a chart's data source has changed. |
| [`refresh_pivot_data(self)`](/cells/python-net/aspose.cells.charts/chart/refresh_pivot_data/#) | Refreshes chart's data from pivot table. |
| [`change_template(self, data)`](/cells/python-net/aspose.cells.charts/chart/change_template/#bytes) | Change chart type with preset template. |
| [`move(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column)`](/cells/python-net/aspose.cells.charts/chart/move/#int-int-int-int) | Moves the chart to a specified location. |
| [`get_actual_size(self)`](/cells/python-net/aspose.cells.charts/chart/get_actual_size/#) | Gets actual size of chart in unit of pixels. |
| [`has_axis(self, aixs_type, is_primary)`](/cells/python-net/aspose.cells.charts/chart/has_axis/#aspose.cells.charts.axistype-bool) | Returns which axes exist on the chart. |
| [`switch_row_column(self)`](/cells/python-net/aspose.cells.charts/chart/switch_row_column/#) | Switches row/column. |
| [`get_chart_data_range(self)`](/cells/python-net/aspose.cells.charts/chart/get_chart_data_range/#) | Gets the data source range of the chart. |
| [`set_chart_data_range(self, area, is_vertical)`](/cells/python-net/aspose.cells.charts/chart/set_chart_data_range/#system.string-bool) | Specifies data range for a chart. |
### Example
The following codes show how to create a chart with .Net codes.
```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType
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
chartIndex = sheet.charts.add(ChartType.COLUMN, 9, 9, 21, 15)
chart = sheet.charts[chartIndex]
chart.set_chart_data_range("A1:B4", True)
chart.show_legend = True
chart.title.text = "Income Analysis"
```
### See Also
* module [`aspose.cells.charts`](..)
* class [`SeriesCollection`](/cells/python-net/aspose.cells.charts/seriescollection)
