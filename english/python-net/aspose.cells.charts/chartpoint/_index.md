---
title: ChartPoint
second_title: Aspose.Cells for Python via .NET API Reference
description: 
type: docs
weight: 90
url: /cells/python-net/aspose.cells.charts/chartpoint/
---

## ChartPoint class

Represents a single point in a series in a chart.

The ChartPoint type exposes the following members:
## Properties
| Name | Description |
| :- | :- |
|explosion|The distance of an open pie slice from the center of the pie chart is expressed as a percentage of the pie diameter.|
|shadow|True if the chartpoint has a shadow.|
|border|Gets the|
|area|Gets the|
|marker|Gets the|
|data_labels|Returns a DataLabels object that represents the data label associated with the point.|
|y_value|Gets or sets the Y value of the chart point.|
|y_value_type|Gets Y value type of the chart point.|
|x_value|Gets or sets the X value of the chart point.|
|x_value_type|Gets X value type of the chart point.|
|shape_properties|Gets the|
|is_in_secondary_plot|Gets or sets a value indicates whether this data points is in the second pie or bar<br/>            on a pie of pie or bar of pie chart|
|shape_x|Gets the x coordinate of the upper left corner in units of 1/4000 of chart's width after calls Chart.Calculate() method.|
|shape_y|Gets the y coordinate of the upper left corner in units of 1/4000 of chart's height after calls Chart.Calculate() method.|
|shape_width|Gets the width in units of 1/4000 of chart's width after calls Chart.Calculate() method.|
|shape_height|Gets the height in units of 1/4000 of chart's height after calls Chart.Calculate() method.|
|shape_x_px|Gets the x coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method.|
|shape_y_px|Gets the y coordinate of the upper left corner in units of pixels after calls Chart.Calculate() method.|
|shape_width_px|Gets the width in units of pixels after calls Chart.Calculate() method.|
|shape_height_px|Gets the height in units of pixels after calls Chart.Calculate() method.|
|border_width_px|Gets the width of border in units of pixels after calls Chart.Calculate() method.|
|radius_px|Gets the radius of bubble, pie or doughnut in units of pixels after calls Chart.Calculate() method.|
|inner_radius_px|Gets the inner radius of doughnut slice in units of pixels after calls Chart.Calculate() method.<br/>            Applies to Doughnut chart.|
|start_angle|Gets the starting angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method.<br/>            Applies to Pie chart.|
|end_angle|Gets the ending angle for the pie section, measured in degrees clockwise from the x-axis after calls Chart.Calculate() method.<br/>            Applies to Pie chart.|
|arc_start_point_x_px|Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method.<br/>            Applies to Pie and Doughnut  chart.|
|arc_start_point_y_px|Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method.<br/>            Applies to Pie and Doughnut  chart.|
|arc_end_point_x_px|Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method.<br/>            Applies to Pie and Doughnut  chart.|
|arc_end_point_y_px|Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method.<br/>            Applies to Pie and Doughnut chart.|
|inner_arc_start_point_x_px|Gets the x coordinate of starting point for the pie section after calls Chart.Calculate() method.<br/>            Applies to Doughnut chart.|
|inner_arc_start_point_y_px|Gets the y coordinate of starting point for the pie section after calls Chart.Calculate() method.<br/>            Applies to Doughnut chart.|
|inner_arc_end_point_x_px|Gets the x coordinate of ending point for the pie section after calls Chart.Calculate() method.<br/>            Applies to Doughnut chart.|
|inner_arc_end_point_y_px|Gets the y coordinate of ending point for the pie section after calls Chart.Calculate() method.<br/>            Applies to Doughnut chart.|
## Methods
| Name | Description |
| :- | :- |
|get_top_point_count()|Gets the number of top points after calls Chart.Calculate() method.|
|get_top_point_x_px(index)|Gets x-coordinate of the top point of shape after calls Chart.Calculate() method.<br/>            Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid and Area3D|
|get_top_point_y_px(index)|Gets y-coordinate of the top point of shape after calls Chart.Calculate() method.<br/>            Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid and Area3D|
|get_bottom_point_count()|Gets the number of bottom points  after calls Chart.Calculate() method.|
|get_bottom_point_x_px(index)|Gets x-coordinate of the bottom point of shape after calls Chart.Calculate() method.<br/>            Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid|
|get_bottom_point_y_px(index)|Gets y-coordinate of the bottom point of shape  after calls Chart.Calculate() method.<br/>            Applies 3D charts: Column3D, Bar3D, Cone, Cylinder, Pyramid|
|get_on_category_axis_point_count()|Gets the number of the points on category axis after calls Chart.Calculate() method. Only applies to area chart.|
|get_on_category_axis_point_x_px(index)|Gets x-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart.|
|get_on_category_axis_point_y_px(index)|Gets y-coordinate of the point on category axis after calls Chart.Calculate() method. Only applies to Area chart.|

### See Also

* namespace [aspose.cells.charts](/cells/python-net/aspose.cells.charts/)
* assembly [Aspose.Cells](/cells/python-net/)

