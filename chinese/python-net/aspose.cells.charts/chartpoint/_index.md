---
title: ChartPoint类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 90
url: /zh/python-net/aspose.cells.charts/chartpoint/
is_root: false
---
## ChartPoint类
表示图表中一系列中的单个点。



ChartPoint 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [explosion](/cells/zh/python-net/aspose.cells.charts/chartpoint/explosion) |开放饼图切片与饼图中心的距离表示为饼图直径的百分比。|
| [shadow](/cells/zh/python-net/aspose.cells.charts/chartpoint/shadow) |如果图表点有阴影则为真。|
| [border](/cells/zh/python-net/aspose.cells.charts/chartpoint/border) |获取 [Line](/cells/zh/python-net/aspose.cells.drawing/line)。|
| [area](/cells/zh/python-net/aspose.cells.charts/chartpoint/area) |获取 [ChartPoint.area](/cells/zh/python-net/aspose.cells.charts/chartpoint#area)。|
| [marker](/cells/zh/python-net/aspose.cells.charts/chartpoint/marker) |获取 [ChartPoint.marker](/cells/zh/python-net/aspose.cells.charts/chartpoint#marker)。|
| [data_labels](/cells/zh/python-net/aspose.cells.charts/chartpoint/data_labels) |返回一个 DataLabels 对象，表示与该点关联的数据标签。|
| [y_value](/cells/zh/python-net/aspose.cells.charts/chartpoint/y_value) |获取或设置图表点的 Y 值。|
| [y_value_type](/cells/zh/python-net/aspose.cells.charts/chartpoint/y_value_type) |获取图表点的 Y 值类型。|
| [x_value](/cells/zh/python-net/aspose.cells.charts/chartpoint/x_value) |获取或设置图表点的 X 值。|
| [x_value_type](/cells/zh/python-net/aspose.cells.charts/chartpoint/x_value_type) |获取图表点的 X 值类型。|
| [shape_properties](/cells/zh/python-net/aspose.cells.charts/chartpoint/shape_properties) |获取 [ShapePropertyCollection](/cells/zh/python-net/aspose.cells.drawing/shapepropertycollection) 对象，该对象保存 ChartPoint 的可视形状属性。|
| [is_in_secondary_plot](/cells/zh/python-net/aspose.cells.charts/chartpoint/is_in_secondary_plot) |获取或设置一个值指示此数据点是否在第二个饼图或条形图中<br/>在一个饼饼图或饼图条上|
| [shape_x](/cells/zh/python-net/aspose.cells.charts/chartpoint/shape_x) |调用Chart.Calculate()方法后，获取图表左上角的x坐标，单位为图表宽度的1/4000。|
| [shape_y](/cells/zh/python-net/aspose.cells.charts/chartpoint/shape_y) |调用Chart.Calculate()方法后，获取图表左上角的y坐标，单位为图表高度的1/4000。|
| [shape_width](/cells/zh/python-net/aspose.cells.charts/chartpoint/shape_width) |在调用 Chart.Calculate() 方法后获取以图表宽度的 1/4000 为单位的宽度。|
| [shape_height](/cells/zh/python-net/aspose.cells.charts/chartpoint/shape_height) |调用 Chart.Calculate() 方法后，以图表高度的 1/4000 为单位获取高度。|
| [shape_x_px](/cells/zh/python-net/aspose.cells.charts/chartpoint/shape_x_px) |调用 Chart.Calculate() 方法后，获取左上角的 x 坐标，以像素为单位。|
| [shape_y_px](/cells/zh/python-net/aspose.cells.charts/chartpoint/shape_y_px) |调用 Chart.Calculate() 方法后，获取左上角的 y 坐标，以像素为单位。|
| [shape_width_px](/cells/zh/python-net/aspose.cells.charts/chartpoint/shape_width_px) |在调用 Chart.Calculate() 方法后获取以像素为单位的宽度。|
| [shape_height_px](/cells/zh/python-net/aspose.cells.charts/chartpoint/shape_height_px) |在调用 Chart.Calculate() 方法后获取以像素为单位的高度。|
| [border_width_px](/cells/zh/python-net/aspose.cells.charts/chartpoint/border_width_px) |调用 Chart.Calculate() 方法后获取以像素为单位的边框宽度。|
| [radius_px](/cells/zh/python-net/aspose.cells.charts/chartpoint/radius_px) |调用 Chart.Calculate() 方法后获取以像素为单位的气泡、饼图或甜甜圈的半径。|
| [inner_radius_px](/cells/zh/python-net/aspose.cells.charts/chartpoint/inner_radius_px) |调用 Chart.Calculate() 方法后以像素为单位获取甜甜圈切片的内半径。<br/>适用于圆环图。|
| [start_angle](/cells/zh/python-net/aspose.cells.charts/chartpoint/start_angle) |获取饼图部分的起始角度，在调用 Chart.Calculate() 方法后从 x 轴顺时针方向测量。<br/>适用于饼图。|
| [end_angle](/cells/zh/python-net/aspose.cells.charts/chartpoint/end_angle) |获取饼图部分的结束角度，在调用 Chart.Calculate() 方法后从 x 轴顺时针测量角度。<br/>适用于饼图。|
| [arc_start_point_x_px](/cells/zh/python-net/aspose.cells.charts/chartpoint/arc_start_point_x_px) |调用 Chart.Calculate() 方法后获取饼图部分起点的 x 坐标。<br/>适用于饼图和圆环图。|
| [arc_start_point_y_px](/cells/zh/python-net/aspose.cells.charts/chartpoint/arc_start_point_y_px) |在调用 Chart.Calculate() 方法后获取饼图部分起点的 y 坐标。<br/>适用于饼图和圆环图。|
| [arc_end_point_x_px](/cells/zh/python-net/aspose.cells.charts/chartpoint/arc_end_point_x_px) |调用 Chart.Calculate() 方法后获取饼图部分终点的 x 坐标。<br/>适用于饼图和圆环图。|
| [arc_end_point_y_px](/cells/zh/python-net/aspose.cells.charts/chartpoint/arc_end_point_y_px) |调用 Chart.Calculate() 方法后获取饼图部分终点的 y 坐标。<br/>适用于饼图和圆环图。|
| [inner_arc_start_point_x_px](/cells/zh/python-net/aspose.cells.charts/chartpoint/inner_arc_start_point_x_px) |调用 Chart.Calculate() 方法后获取饼图部分起点的 x 坐标。<br/>适用于圆环图。|
| [inner_arc_start_point_y_px](/cells/zh/python-net/aspose.cells.charts/chartpoint/inner_arc_start_point_y_px) |在调用 Chart.Calculate() 方法后获取饼图部分起点的 y 坐标。<br/>适用于圆环图。|
| [inner_arc_end_point_x_px](/cells/zh/python-net/aspose.cells.charts/chartpoint/inner_arc_end_point_x_px) |调用 Chart.Calculate() 方法后获取饼图部分终点的 x 坐标。<br/>适用于圆环图。|
| [inner_arc_end_point_y_px](/cells/zh/python-net/aspose.cells.charts/chartpoint/inner_arc_end_point_y_px) |调用 Chart.Calculate() 方法后获取饼图部分终点的 y 坐标。<br/>适用于圆环图。|


### 方法
|方法|描述|
| :- | :- |
| [get_top_point_count()](/cells/zh/python-net/aspose.cells.charts/chartpoint/get_top_point_count/#) |调用 Chart.Calculate() 方法后获取最高点数。|
| [get_top_point_x_px(index)](/cells/zh/python-net/aspose.cells.charts/chartpoint/get_top_point_x_px/#int) |调用 Chart.Calculate() 方法后获取形状顶点的 x 坐标。<br/>适用 3D 图表：Column3D、Bar3D、Cone、Cylinder、Pyramid 和 Area3D|
| [get_top_point_y_px(index)](/cells/zh/python-net/aspose.cells.charts/chartpoint/get_top_point_y_px/#int) |调用 Chart.Calculate() 方法后获取形状顶点的 y 坐标。<br/>适用 3D 图表：Column3D、Bar3D、Cone、Cylinder、Pyramid 和 Area3D|
| [get_bottom_point_count()](/cells/zh/python-net/aspose.cells.charts/chartpoint/get_bottom_point_count/#) |调用 Chart.Calculate() 方法后获取底部点数。|
| [get_bottom_point_x_px(index)](/cells/zh/python-net/aspose.cells.charts/chartpoint/get_bottom_point_x_px/#int) |调用 Chart.Calculate() 方法后获取形状底点的 x 坐标。<br/>适用 3D 图表：Column3D、Bar3D、Cone、Cylinder、Pyramid|
| [get_bottom_point_y_px(index)](/cells/zh/python-net/aspose.cells.charts/chartpoint/get_bottom_point_y_px/#int) |调用 Chart.Calculate() 方法后获取形状底点的 y 坐标。<br/>适用 3D 图表：Column3D、Bar3D、Cone、Cylinder、Pyramid|
| [get_on_category_axis_point_count()](/cells/zh/python-net/aspose.cells.charts/chartpoint/get_on_category_axis_point_count/#) |调用 Chart.Calculate() 方法后获取类别轴上的点数。仅适用于面积图。|
| [get_on_category_axis_point_x_px(index)](/cells/zh/python-net/aspose.cells.charts/chartpoint/get_on_category_axis_point_x_px/#int) |调用 Chart.Calculate() 方法后获取类别轴上点的 x 坐标。仅适用于面积图。|
| [get_on_category_axis_point_y_px(index)](/cells/zh/python-net/aspose.cells.charts/chartpoint/get_on_category_axis_point_y_px/#int) |调用 Chart.Calculate() 方法后获取类别轴上点的 y 坐标。仅适用于面积图。|



### 例子

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

### 也可以看看
* 模块 [aspose.cells.charts](..)
* 类 [Line](/cells/zh/python-net/aspose.cells.drawing/line)
* 类 [ShapePropertyCollection](/cells/zh/python-net/aspose.cells.drawing/shapepropertycollection)
