---
title: Chart
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 30
url: /cells/python-net/aspose.cells.charts/chart/
---

## Chart class

Encapsulates the object that represents a single Excel chart.

The Chart type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|style|Gets and sets the builtin style.|
|chart_object|Represents the chartShape;|
|hide_pivot_field_buttons|Indicates whether hide the pivot chart field buttons only when the chart is PivotChart.|
|pivot_options|Specifies the pivot controls that appear on the chart|
|pivot_source|The source is the data of the pivotTable.<br/>            If PivotSource is not empty ,the chart is PivotChart.|
|plot_by|Gets and sets whether plot by row or column.|
|plot_empty_cells_type|Gets and sets  how to plot the empty cells.|
|plot_visible_cells|Indicates whether only plot visible cells.|
|display_na_as_blank|Indicates whether displaying #N/A as blank value.|
|name|Gets and sets the name of the chart.|
|size_with_window|True if Microsoft Excel resizes the chart to match the size of the chart sheet window.|
|worksheet|Gets the worksheet which contains this chart.|
|shapes|Returns all drawing shapes in this chart.|
|print_size|Gets and sets the printed chart size.|
|type|Gets or sets a chart's type.|
|n_series|Gets a [SeriesCollection](/cells/python-net/aspose.cells.charts/seriescollection/) collection representing the data series in the chart.|
|title|Gets the chart's title.|
|sub_title|Gets the chart's sub-title.<br/>            Only for ODS format file.|
|plot_area|Gets the chart's plot area which includes axis tick labels.|
|chart_area|Gets the chart area in the worksheet.|
|category_axis|Gets the chart's X axis.|
|value_axis|Gets the chart's Y axis.|
|second_value_axis|Gets the chart's second Y axis.|
|second_category_axis|Gets the chart's second X axis.|
|series_axis|Gets the chart's series axis.|
|legend|Gets the chart legend.|
|chart_data_table|Represents the chart data table.|
|show_legend|Gets or sets a value indicating whether the chart legend will be displayed. Default is true.|
|is_rectangular_cornered|Gets or sets a value indicating whether the chart area is rectangular cornered.<br/>            Default is true.|
|show_data_table|Gets or sets a value indicating whether the chart displays a data table.|
|first_slice_angle|Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.|
|gap_width|Returns or sets the space between bar or column clusters, as a percentage of the bar or column width.<br/>            The value of this property must be between 0 and 500.|
|gap_depth|Gets or sets the distance between the data series in a 3-D chart, as a percentage of the marker width.<br/>            The value of this property must be between 0 and 500.|
|floor|Returns a [floor](/cells/python-net/aspose.cells.charts/chart/) object that represents the walls of a 3-D chart.|
|walls|Returns a [walls](/cells/python-net/aspose.cells.charts/chart/) object that represents the walls of a 3-D chart.|
|back_wall|Returns a [walls](/cells/python-net/aspose.cells.charts/chart/) object that represents the back wall of a 3-D chart.|
|side_wall|Returns a [walls](/cells/python-net/aspose.cells.charts/chart/) object that represents the side wall of a 3-D chart.|
|walls_and_gridlines_2d|True if gridlines are drawn two-dimensionally on a 3-D chart.|
|rotation_angle|Represents the rotation of the 3-D chart view (the rotation of the plot area around the z-axis, in degrees).|
|elevation|Represents the elevation of the 3-D chart view, in degrees.|
|right_angle_axes|True if the chart axes are at right angles. Applies only for 3-D charts(except Column3D and 3-D Pie Charts).|
|auto_scaling|True if Microsoft Excel scales a 3-D chart so that it's closer in size to the equivalent 2-D chart. <br/>            The RightAngleAxes property must be True.|
|height_percent|Returns or sets the height of a 3-D chart as a percentage of the chart width (between 5 and 500 percent).|
|perspective|Returns or sets the perspective for the 3-D chart view. Must be between 0 and 100.<br/>            This property is ignored if the RightAngleAxes property is True.|
|is_3d|Indicates whether the chart is a 3d chart.|
|depth_percent|Represents the depth of a 3-D chart as a percentage of the chart width (between 20 and 2000 percent).|
|actual_chart_size|Gets actual size of chart in unit of pixels.|
|placement|Represents the way the chart is attached to the cells below it.|
|page_setup|Represents the page setup description in this chart.|
|line|Gets the line.|
## Methods
| Name | Description |
| :- | :- |
|to_image(image_file)|Creates the chart image and saves it to a file.<br/>            The extension of the file name determines the format of the image.|
|to_image(image_file, image_type)|Creates the chart image and saves it to a file in the specified image type.|
|to_image(image_file, jpeg_quality)|  |
|to_image(stream, jpeg_quality)|  |
|to_image(stream, image_type)|Creates the chart image and saves it to a stream in the specified format.|
|to_image(image_file, options)|Creates the chart image and saves it to a file.<br/>             The extension of the file name determines the format of the image.|
|to_image(stream, options)|Creates the chart image and saves it to a stream in the specified format.|
|to_pdf(file_name)|Saves the chart to a pdf file.|
|to_pdf(file_name, desired_page_width, desired_page_height, h_alignment_type, v_alignment_type)|Saves the chart to a pdf file.|
|to_pdf(stream)|Creates the chart pdf and saves it to a stream.|
|to_pdf(stream, desired_page_width, desired_page_height, h_alignment_type, v_alignment_type)|Creates the chart pdf and saves it to a stream.|
|is_chart_data_changed()|Detects if a chart's data source has changed.|
|refresh_pivot_data()|Refreshes pivot chart's data  from it's pivot data source.|
|change_template(data)|Change chart type with preset template.|
|move(upper_left_row, upper_left_column, lower_right_row, lower_right_column)|Moves the chart to a specified location.|
|calculate()|Calculates the custom position of plot area, axes if the position of them are auto assigned.|
|get_actual_size()|Gets actual size of chart in unit of pixels.|
|has_axis(aixs_type, is_primary)|Returns which axes exist on the chart.|
|switch_row_column()|Switches row/column.|
|get_chart_data_range()|Gets the data source range of the chart.|
|set_chart_data_range(area, is_vertical)|Specifies data range for a chart.|

### See Also

* namespace [aspose.cells.charts](/cells/python-net/aspose.cells.charts/)
* assembly [Aspose.Cells](/cells/python-net/)

