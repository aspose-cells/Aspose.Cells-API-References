---
title: Chart类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 30
url: /zh/python-net/aspose.cells.charts/chart/
is_root: false
---
## Chart类
封装表示单个 Excel 图表的对象。



Chart 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [style](/cells/zh/python-net/aspose.cells.charts/chart/style) |获取和设置内置样式。|
| [chart_object](/cells/zh/python-net/aspose.cells.charts/chart/chart_object) |代表图表形状；|
| [hide_pivot_field_buttons](/cells/zh/python-net/aspose.cells.charts/chart/hide_pivot_field_buttons) |指示是否仅在图表为数据透视图时隐藏数据透视图字段按钮。|
| [pivot_options](/cells/zh/python-net/aspose.cells.charts/chart/pivot_options) |指定显示在图表上的数据透视控件|
| [pivot_source](/cells/zh/python-net/aspose.cells.charts/chart/pivot_source) |源是数据透视表的数据。<br/>如果 PivotSource 不为空，则图表为 PivotChart。|
| [plot_by](/cells/zh/python-net/aspose.cells.charts/chart/plot_by) |获取和设置是按行还是按列绘制。|
| [plot_empty_cells_type](/cells/zh/python-net/aspose.cells.charts/chart/plot_empty_cells_type) |获取并设置如何绘制空单元格。|
| [plot_visible_cells](/cells/zh/python-net/aspose.cells.charts/chart/plot_visible_cells) |指示是否仅绘制可见单元格。|
| [plot_visible_cells_only](/cells/zh/python-net/aspose.cells.charts/chart/plot_visible_cells_only) |指示是否仅绘制可见单元格。|
| [display_na_as_blank](/cells/zh/python-net/aspose.cells.charts/chart/display_na_as_blank) |指示是否将#N/A 显示为空白值。|
| [name](/cells/zh/python-net/aspose.cells.charts/chart/name) |获取和设置图表的名称。|
| [size_with_window](/cells/zh/python-net/aspose.cells.charts/chart/size_with_window) |如果 Microsoft Excel 调整图表大小以匹配图表工作表窗口的大小，则为真。|
| [worksheet](/cells/zh/python-net/aspose.cells.charts/chart/worksheet) |获取包含此图表的工作表。|
| [shapes](/cells/zh/python-net/aspose.cells.charts/chart/shapes) |返回此图表中的所有绘图形状。|
| [print_size](/cells/zh/python-net/aspose.cells.charts/chart/print_size) |获取和设置打印的图表大小。|
| [type](/cells/zh/python-net/aspose.cells.charts/chart/type) |获取或设置图表的类型。|
| [n_series](/cells/zh/python-net/aspose.cells.charts/chart/n_series) |获取表示图表中数据系列的 [SeriesCollection](/cells/zh/python-net/aspose.cells.charts/seriescollection) 集合。|
| [title](/cells/zh/python-net/aspose.cells.charts/chart/title) |获取图表的标题。|
| [sub_title](/cells/zh/python-net/aspose.cells.charts/chart/sub_title) |获取图表的副标题。<br/>仅适用于 ODS 格式文件。|
| [plot_area](/cells/zh/python-net/aspose.cells.charts/chart/plot_area) |获取图表的绘图区域，其中包括轴刻度标签。|
| [chart_area](/cells/zh/python-net/aspose.cells.charts/chart/chart_area) |获取工作表中的图表区域。|
| [category_axis](/cells/zh/python-net/aspose.cells.charts/chart/category_axis) |获取图表的 X 轴。|
| [value_axis](/cells/zh/python-net/aspose.cells.charts/chart/value_axis) |获取图表的 Y 轴。|
| [second_value_axis](/cells/zh/python-net/aspose.cells.charts/chart/second_value_axis) |获取图表的第二个 Y 轴。|
| [second_category_axis](/cells/zh/python-net/aspose.cells.charts/chart/second_category_axis) |获取图表的第二个 X 轴。|
| [series_axis](/cells/zh/python-net/aspose.cells.charts/chart/series_axis) |获取图表的系列轴。|
| [legend](/cells/zh/python-net/aspose.cells.charts/chart/legend) |获取图表图例。|
| [chart_data_table](/cells/zh/python-net/aspose.cells.charts/chart/chart_data_table) |代表图表数据表。|
| [show_legend](/cells/zh/python-net/aspose.cells.charts/chart/show_legend) |获取或设置一个值，该值指示是否显示图表图例。默认为真。|
| [is_rectangular_cornered](/cells/zh/python-net/aspose.cells.charts/chart/is_rectangular_cornered) |获取或设置一个值，该值指示图表区域是否为矩形角。<br/>默认为真。|
| [show_data_table](/cells/zh/python-net/aspose.cells.charts/chart/show_data_table) |获取或设置一个值，该值指示图表是否显示数据表。|
| [first_slice_angle](/cells/zh/python-net/aspose.cells.charts/chart/first_slice_angle) |获取或设置第一个饼图或圆环图切片的角度，以度为单位（从垂直方向顺时针方向）。仅适用于饼图、3-D 饼图和圆环图，0 到 360。|
| [gap_width](/cells/zh/python-net/aspose.cells.charts/chart/gap_width) |返回或设置条形或列簇之间的空间，作为条形或列宽的百分比。<br/>此属性的值必须介于 0 和 500 之间。|
| [gap_depth](/cells/zh/python-net/aspose.cells.charts/chart/gap_depth) |获取或设置 3-D 图表中数据系列之间的距离，以标记宽度的百分比表示。<br/>此属性的值必须介于 0 和 500 之间。|
| [floor](/cells/zh/python-net/aspose.cells.charts/chart/floor) |返回代表 3-D 图表的墙壁的 [Chart.floor](/cells/zh/python-net/aspose.cells.charts/chart#floor) 对象。|
| [walls](/cells/zh/python-net/aspose.cells.charts/chart/walls) |返回代表 3-D 图表的墙壁的 [Chart.walls](/cells/zh/python-net/aspose.cells.charts/chart#walls) 对象。|
| [back_wall](/cells/zh/python-net/aspose.cells.charts/chart/back_wall) |返回代表 3-D 图表后墙的 [Chart.walls](/cells/zh/python-net/aspose.cells.charts/chart#walls) 对象。|
| [side_wall](/cells/zh/python-net/aspose.cells.charts/chart/side_wall) |返回代表 3-D 图表侧壁的 [Chart.walls](/cells/zh/python-net/aspose.cells.charts/chart#walls) 对象。|
| [walls_and_gridlines_2d](/cells/zh/python-net/aspose.cells.charts/chart/walls_and_gridlines_2d) |如果在 3-D 图表上以二维方式绘制网格线，则为真。|
| [rotation_angle](/cells/zh/python-net/aspose.cells.charts/chart/rotation_angle) |表示 3-D 图表视图的旋转（绘图区域围绕 z 轴的旋转，以度为单位）。|
| [elevation](/cells/zh/python-net/aspose.cells.charts/chart/elevation) |表示 3-D 图表视图的高度，以度为单位。|
| [right_angle_axes](/cells/zh/python-net/aspose.cells.charts/chart/right_angle_axes) |如果图表轴成直角则为真。仅适用于 3-D 图表（Column3D 和 3-D 饼图除外）。|
| [auto_scaling](/cells/zh/python-net/aspose.cells.charts/chart/auto_scaling) |如果 Microsoft Excel 缩放 3-D 图表，使其在大小上更接近等效的 2-D 图表，则为真。<br/> RightAngleAxes 属性必须为 True。|
| [height_percent](/cells/zh/python-net/aspose.cells.charts/chart/height_percent) |返回或设置 3-D 图表的高度占图表宽度的百分比（介于 5% 和 500% 之间）。|
| [perspective](/cells/zh/python-net/aspose.cells.charts/chart/perspective) |返回或设置 3-D 图表视图的透视图。必须介于 0 和 100 之间。<br/>如果 RightAngleAxes 属性为 True，则忽略此属性。|
| [is_3d](/cells/zh/python-net/aspose.cells.charts/chart/is_3d) |指示图表是否为 3d 图表。|
| [depth_percent](/cells/zh/python-net/aspose.cells.charts/chart/depth_percent) |表示 3-D 图表的深度占图表宽度的百分比（介于 20% 和 2000% 之间）。|
| [actual_chart_size](/cells/zh/python-net/aspose.cells.charts/chart/actual_chart_size) |以像素为单位获取图表的实际大小。|
| [placement](/cells/zh/python-net/aspose.cells.charts/chart/placement) |表示图表附加到其下方单元格的方式。|
| [page_setup](/cells/zh/python-net/aspose.cells.charts/chart/page_setup) |表示此图表中的页面设置说明。|
| [line](/cells/zh/python-net/aspose.cells.charts/chart/line) |获取线路。|


### 方法
|方法|描述|
| :- | :- |
| [to_image(image_file)](/cells/zh/python-net/aspose.cells.charts/chart/to_image/#str) |创建图表图像并将其保存到文件中。<br/>文件名的扩展名决定了图像的格式。|
| [to_image(image_file, image_type)](/cells/zh/python-net/aspose.cells.charts/chart/to_image/#str-aspose.cells.drawing.ImageType) |创建图表图像并将其保存到指定图像类型的文件中。|
| [to_image(image_file, jpeg_quality)](/cells/zh/python-net/aspose.cells.charts/chart/to_image/#str-int) |创建图表图像并将其保存到 Jpeg 格式的文件中。|
| [to_image(stream, jpeg_quality)](/cells/zh/python-net/aspose.cells.charts/chart/to_image/#io.RawIOBase-int) |创建图表图像并将其保存到 Jpeg 格式的流中。|
| [to_image(stream, image_type)](/cells/zh/python-net/aspose.cells.charts/chart/to_image/#io.RawIOBase-aspose.cells.drawing.ImageType) |创建图表图像并将其保存到指定格式的流中。|
| [to_image(image_file, options)](/cells/zh/python-net/aspose.cells.charts/chart/to_image/#str-aspose.cells.rendering.ImageOrPrintOptions) |创建图表图像并将其保存到文件中。<br/>文件名的扩展名决定了图像的格式。|
| [to_image(stream, options)](/cells/zh/python-net/aspose.cells.charts/chart/to_image/#io.RawIOBase-aspose.cells.rendering.ImageOrPrintOptions) |创建图表图像并将其保存到指定格式的流中。|
| [to_pdf(file_name)](/cells/zh/python-net/aspose.cells.charts/chart/to_pdf/#str) |将图表保存为 pdf 文件。|
| [to_pdf(file_name, desired_page_width, desired_page_height, h_alignment_type, v_alignment_type)](/cells/zh/python-net/aspose.cells.charts/chart/to_pdf/#str-float-float-PageLayoutAlignmentType-PageLayoutAlignmentType) |将图表保存为 pdf 文件。|
| [to_pdf(stream)](/cells/zh/python-net/aspose.cells.charts/chart/to_pdf/#io.RawIOBase) |创建图表 pdf 并将其保存到流中。|
| [to_pdf(stream, desired_page_width, desired_page_height, h_alignment_type, v_alignment_type)](/cells/zh/python-net/aspose.cells.charts/chart/to_pdf/#io.RawIOBase-float-float-PageLayoutAlignmentType-PageLayoutAlignmentType) |创建图表 pdf 并将其保存到流中。|
| [is_chart_data_changed()](/cells/zh/python-net/aspose.cells.charts/chart/is_chart_data_changed/#) |检测图表的数据源是否已更改。|
| [refresh_pivot_data()](/cells/zh/python-net/aspose.cells.charts/chart/refresh_pivot_data/#) |从数据透视数据源刷新数据透视图表的数据。|
| [change_template(data)](/cells/zh/python-net/aspose.cells.charts/chart/change_template/#bytes) |使用预设模板更改图表类型。|
| [move(upper_left_row, upper_left_column, lower_right_row, lower_right_column)](/cells/zh/python-net/aspose.cells.charts/chart/move/#int-int-int-int) |将图表移动到指定位置。|
| [calculate()](/cells/zh/python-net/aspose.cells.charts/chart/calculate/#) |计算绘图区域的自定义位置，如果它们的位置是自动分配的，则轴。|
| [get_actual_size()](/cells/zh/python-net/aspose.cells.charts/chart/get_actual_size/#) |以像素为单位获取图表的实际大小。|
| [has_axis(aixs_type, is_primary)](/cells/zh/python-net/aspose.cells.charts/chart/has_axis/#AxisType-bool) |返回图表上存在哪些轴。|
| [switch_row_column()](/cells/zh/python-net/aspose.cells.charts/chart/switch_row_column/#) |切换行/列。|
| [get_chart_data_range()](/cells/zh/python-net/aspose.cells.charts/chart/get_chart_data_range/#) |获取图表的数据源范围。|
| [set_chart_data_range(area, is_vertical)](/cells/zh/python-net/aspose.cells.charts/chart/set_chart_data_range/#str-bool) |指定图表的数据范围。|



### 例子

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

### 也可以看看
* 模块 [aspose.cells.charts](..)
* 类 [SeriesCollection](/cells/zh/python-net/aspose.cells.charts/seriescollection)
