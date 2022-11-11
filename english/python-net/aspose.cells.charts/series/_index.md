---
title: Series
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 230
url: /cells/python-net/aspose.cells.charts/series/
---

## Series class

Encapsulates the object that represents a single data series in a chart.

The Series type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|layout_properties|Represents the properties of layout.|
|points|Gets the collection of points in a series in a chart.|
|area|Represents the background area of Series object.|
|border|Represents border of Series object.|
|name|Gets or sets the name of the data series.|
|display_name|Gets the series's name that displays on the chart graph.|
|count_of_data_values|Gets the number of the data values.|
|is_vertical_values|Indicates whether the data source is vertical.|
|values|Represents the data of the chart series.|
|values_format_code|Represents format code of Values‘s NumberList.|
|x_values|Represents the x values of the chart series.|
|bubble_sizes|Gets or sets the bubble sizes values of the chart series.|
|trend_lines|Returns an object that represents a collection of all the trendlines for the series.|
|smooth|Represents curve smoothing. <br/>            True if curve smoothing is turned on for the line chart or scatter chart.<br/>            Applies only to line and scatter connected by lines charts.|
|shadow|True if the series has a shadow.|
|has_3d_effect|True if the series has a three-dimensional appearance. <br/>            Applies only to bubble charts.|
|bar_3d_shape_type|Gets or sets the 3D shape type used with the 3-D bar or column chart.|
|bar_shape|Gets or sets the 3D shape type used with the 3-D bar or column chart.|
|data_labels|Represents the DataLabels object for the specified ASeries.|
|type|Gets or sets a data series' type.|
|marker|Gets the|
|plot_on_second_axis|Indicates if this series is plotted on second value axis.|
|x_error_bar|Represents X direction error bar of the series.|
|y_error_bar|Represents Y direction error bar of the series.|
|has_hi_lo_lines|True if the line chart has high-low lines. <br/>             Applies only to line charts.|
|hi_lo_lines|Returns a HiLoLines object that represents the high-low lines for a series on a line chart. <br/>            Applies only to line charts.|
|has_series_lines|True if a stacked column chart or bar chart has series lines or<br/>            if a Pie of Pie chart or Bar of Pie chart has connector lines between the two sections. <br/>            Applies only to stacked column charts, bar charts, Pie of Pie charts, or Bar of Pie charts.|
|series_lines|Returns a SeriesLines object that represents the series lines for a stacked bar chart or a stacked column chart.<br/>            Applies only to stacked bar and stacked column charts.|
|has_drop_lines|True if the chart has drop lines.<br/>            Applies only to line chart or area charts.|
|drop_lines|Returns a [Line](/cells/python-net/aspose.cells.drawing/line/) object that represents the drop lines for a series on the line chart or area chart.<br/>            Applies only to line chart or area charts.|
|has_up_down_bars|True if a line chart has up and down bars.<br/>            Applies only to line charts.|
|up_bars|Returns an DropBars object that represents the up bars on a line chart.<br/>            Applies only to line charts.|
|down_bars|Returns a [DropBars](/cells/python-net/aspose.cells.charts/dropbars/) object that represents the down bars on a line chart.<br/>            Applies only to line charts.|
|is_color_varied|Represents if the color of points is varied. <br/>            The chart must contain only one series.|
|gap_width|Returns or sets the space between bar or column clusters, as a percentage of the bar or column width.<br/>            The value of this property must be between 0 and 500.|
|first_slice_angle|Gets or sets the angle of the first pie-chart or doughnut-chart slice, in degrees (clockwise from vertical). <br/>            Applies only to pie, 3-D pie, and doughnut charts, 0 to 360.|
|overlap|Specifies how bars and columns are positioned.<br/>            Can be a value between – 100 and 100. <br/>            Applies only to 2-D bar and 2-D column charts.|
|second_plot_size|Returns or sets the size of the secondary section of either a pie of pie chart or a bar of pie chart, <br/>            as a percentage of the size of the primary pie.<br/>            Can be a value from 5 to 200.|
|split_type|Returns or sets a value that how to determine which data points are in the second pie or bar on a pie of pie or bar of<br/>            pie chart.|
|split_value|Returns or sets a value that shall be used to determine which data points are in the second pie or bar on<br/>            a pie of pie or bar of pie chart.|
|is_auto_split|Indicates whether the threshold value is automatic.|
|bubble_scale|Gets or sets the scale factor for bubbles in the specified chart group. <br/>            It can be an integer value from 0 (zero) to 300, <br/>            corresponding to a percentage of the default size.<br/>            Applies only to bubble charts.|
|size_represents|Gets or sets what the bubble size represents on a bubble chart.|
|show_negative_bubbles|True if negative bubbles are shown for the chart group. Valid only for bubble charts.|
|doughnut_hole_size|Returns or sets the size of the hole in a doughnut chart group. <br/>            The hole size is expressed as a percentage of the chart size, between 10 and 90 percent.|
|explosion|The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.|
|has_radar_axis_labels|True if a radar chart has category axis labels. Applies only to radar charts.|
|has_leader_lines|True if the series has leader lines.|
|leader_lines|Represents leader lines on a chart. Leader lines connect data labels to data points. <br/>            This object isn’t a collection; there’s no object that represents a single leader line.|
|legend_entry|Gets the legend entry according to this series.|
|shape_properties|Gets the|
## Methods
| Name | Description |
| :- | :- |
|move(count)|Moves the series up or down.|

### See Also

* namespace [aspose.cells.charts](/cells/python-net/aspose.cells.charts/)
* assembly [Aspose.Cells](/cells/python-net/)

