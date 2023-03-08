---
title: SparklineGroup类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 280
url: /zh/python-net/aspose.cells.charts/sparklinegroup/
is_root: false
---
##  SparklineGroup类
[Sparkline](/cells/zh/python-net/aspose.cells.charts/sparkline) 被组织到迷你图组中。 SparklineGroup 包含可变数量的迷你图项目。
迷你图组指定迷你图的类型、显示设置和轴设置。



SparklineGroup 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [preset_style](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/preset_style) |获取和设置迷你图组的预设样式类型。|
| [sparkline_collection](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/sparkline_collection) |获取 [Sparkline](/cells/zh/python-net/aspose.cells.charts/sparkline) 对象的集合。|
| [sparklines](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/sparklines) |获取 [Sparkline](/cells/zh/python-net/aspose.cells.charts/sparkline) 对象的集合。|
| [type](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/type) |指示迷你图组的迷你图类型。|
| [plot_empty_cells_type](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/plot_empty_cells_type) |指示如何绘制空单元格。|
| [display_hidden](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/display_hidden) |指示是否在隐藏的行和列中显示数据。|
| [show_high_point](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/show_high_point) |指示是否突出显示迷你图组中数据的最高点。|
| [high_point_color](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/high_point_color) |获取和设置迷你图组中数据最高点的颜色。|
| [show_low_point](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/show_low_point) |指示是否突出显示迷你图组中数据的最低点。|
| [low_point_color](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/low_point_color) |获取和设置迷你图组中数据最低点的颜色。|
| [show_negative_points](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/show_negative_points) |指示是否使用不同的颜色或标记突出显示迷你图组中的负值。|
| [negative_points_color](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/negative_points_color) |获取和设置迷你图组中负值的颜色。|
| [show_first_point](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/show_first_point) |指示是否突出显示迷你图组中的第一个数据点。|
| [first_point_color](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/first_point_color) |获取和设置迷你图组中第一个数据点的颜色。|
| [show_last_point](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/show_last_point) |指示是否突出显示迷你图组中的最后一个数据点。|
| [last_point_color](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/last_point_color) |获取和设置迷你图组中最后一个数据点的颜色。|
| [show_markers](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/show_markers) |指示是否突出显示迷你图组中每条线迷你图中的每个点。|
| [markers_color](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/markers_color) |获取和设置迷你图组中每条线迷你图中点的颜色。|
| [series_color](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/series_color) |获取和设置迷你图组中迷你图的颜色。|
| [plot_right_to_left](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/plot_right_to_left) |指示绘图数据是否从右到左。|
| [line_weight](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/line_weight) |获取和设置迷你图组中每条线条迷你图的线宽，单位为点。|
| [horizontal_axis_color](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/horizontal_axis_color) |获取和设置迷你图组中水平轴的颜色。|
| [show_horizontal_axis](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/show_horizontal_axis) |指示是否显示迷你图水平轴。<br/>如果迷你图具有穿过零轴的数据，则会出现水平轴。|
| [horizontal_axis_date_range](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/horizontal_axis_date_range) |表示包含迷你图数据的日期值的范围。|
| [vertical_axis_max_value_type](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/vertical_axis_max_value_type) |表示垂直轴最大值类型。|
| [vertical_axis_max_value](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/vertical_axis_max_value) |获取和设置垂直轴的自定义最大值。|
| [vertical_axis_min_value_type](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/vertical_axis_min_value_type) |表示纵轴最小值类型。|
| [vertical_axis_min_value](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/vertical_axis_min_value) |获取和设置垂直轴的自定义最小值。|


### 方法
|方法|描述|
| :- | :- |
| [reset_ranges(data_range, is_vertical, location_range)](/cells/zh/python-net/aspose.cells.charts/sparklinegroup/reset_ranges/#str-bool-CellArea) |重置迷你图组的数据范围和位置范围。<br/>此方法将清除组中的原始迷你图项目并为新范围创建新的迷你图项目。|



### 例子

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
idx = sheet.sparkline_group_collection.add(SparklineType.LINE, "A1:D1", False, ca)
group = sheet.sparkline_group_collection[idx]
group.sparkline_collection.add(sheet.name + "!A1:D1", 0, 4)
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

### 也可以看看
* 模块 [aspose.cells.charts](..)
* 类 [Sparkline](/cells/zh/python-net/aspose.cells.charts/sparkline)
