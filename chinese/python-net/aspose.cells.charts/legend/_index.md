---
title: Legend类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 170
url: /zh/python-net/aspose.cells.charts/legend/
is_root: false
---
## Legend类
封装表示图表图例的对象。



**继承：** [Legend](/cells/python-net/aspose.cells.charts/legend) → 
[ChartTextFrame](/cells/python-net/aspose.cells.charts/charttextframe) → 
[ChartFrame](/cells/zh/python-net/aspose.cells.charts/chartframe)



Legend 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [is_inner_mode](/cells/zh/python-net/aspose.cells.charts/legend/is_inner_mode) |指示绘图区域大小是否包括刻度线和轴标签。<br/> False 指定大小应确定绘图区域、刻度线和轴标签的大小。|
| [border](/cells/zh/python-net/aspose.cells.charts/legend/border) |获取 [Line](/cells/zh/python-net/aspose.cells.drawing/line)。|
| [area](/cells/zh/python-net/aspose.cells.charts/legend/area) |获取 [ChartFrame.area](/cells/zh/python-net/aspose.cells.charts/chartframe#area)。|
| [text_font](/cells/zh/python-net/aspose.cells.charts/legend/text_font) |获取指定 ChartFrame 对象的 [ChartFrame.font](/cells/zh/python-net/aspose.cells.charts/chartframe#font) 对象。|
| [text_options](/cells/zh/python-net/aspose.cells.charts/legend/text_options) |获取和设置文本的选项。|
| [font](/cells/zh/python-net/aspose.cells.charts/legend/font) |获取指定 ChartFrame 对象的 [ChartFrame.font](/cells/zh/python-net/aspose.cells.charts/chartframe#font) 对象。|
| [auto_scale_font](/cells/zh/python-net/aspose.cells.charts/legend/auto_scale_font) |如果对象中的文本在对象大小更改时更改字体大小，则为真。|
| [background_mode](/cells/zh/python-net/aspose.cells.charts/legend/background_mode) |获取和设置背景的显示方式|
| [background](/cells/zh/python-net/aspose.cells.charts/legend/background) |获取和设置背景的显示方式|
| [is_automatic_size](/cells/zh/python-net/aspose.cells.charts/legend/is_automatic_size) |指示图表框是否自动调整大小。|
| [x](/cells/zh/python-net/aspose.cells.charts/legend/x) |获取或设置图表区域左上角的 x 坐标，单位为 1/4000。|
| [y](/cells/zh/python-net/aspose.cells.charts/legend/y) |获取或设置图表区域左上角的y坐标，单位为1/4000。|
| [height](/cells/zh/python-net/aspose.cells.charts/legend/height) |获取或设置以图表区域的 1/4000 为单位的框架高度。|
| [width](/cells/zh/python-net/aspose.cells.charts/legend/width) |获取或设置以图表区域的 1/4000 为单位的框架宽度。|
| [shadow](/cells/zh/python-net/aspose.cells.charts/legend/shadow) |如果框架有阴影，则为真。|
| [shape_properties](/cells/zh/python-net/aspose.cells.charts/legend/shape_properties) |获取 [ChartFrame.shape_properties](/cells/zh/python-net/aspose.cells.charts/chartframe#shape_properties) 对象。|
| [is_default_pos_be_set](/cells/zh/python-net/aspose.cells.charts/legend/is_default_pos_be_set) |指示是否设置了默认位置（DefaultX、DefaultY、DefaultWidth 和 DefaultHeight）。|
| [default_x](/cells/zh/python-net/aspose.cells.charts/legend/default_x) |表示默认位置的x|
| [default_y](/cells/zh/python-net/aspose.cells.charts/legend/default_y) |代表默认位置的y|
| [default_width](/cells/zh/python-net/aspose.cells.charts/legend/default_width) |表示默认位置的宽度|
| [default_height](/cells/zh/python-net/aspose.cells.charts/legend/default_height) |表示默认位置的高度|
| [is_auto_text](/cells/zh/python-net/aspose.cells.charts/legend/is_auto_text) |表示文本是自动生成的。|
| [is_deleted](/cells/zh/python-net/aspose.cells.charts/legend/is_deleted) |指示是否删除此数据标签。|
| [text_horizontal_alignment](/cells/zh/python-net/aspose.cells.charts/legend/text_horizontal_alignment) |获取和设置文本水平对齐方式。|
| [text_vertical_alignment](/cells/zh/python-net/aspose.cells.charts/legend/text_vertical_alignment) |获取或设置文本的文本垂直对齐方式。|
| [rotation_angle](/cells/zh/python-net/aspose.cells.charts/legend/rotation_angle) |表示文本旋转角度。|
| [is_automatic_rotation](/cells/zh/python-net/aspose.cells.charts/legend/is_automatic_rotation) |指示图表的文本是否自动旋转。|
| [text](/cells/zh/python-net/aspose.cells.charts/legend/text) |获取或设置框架标题的文本。|
| [linked_source](/cells/zh/python-net/aspose.cells.charts/legend/linked_source) |获取和设置对工作表的引用。|
| [text_direction](/cells/zh/python-net/aspose.cells.charts/legend/text_direction) |表示文本阅读顺序。|
| [reading_order](/cells/zh/python-net/aspose.cells.charts/legend/reading_order) |表示文本阅读顺序。|
| [direction_type](/cells/zh/python-net/aspose.cells.charts/legend/direction_type) |获取和设置文本的方向。|
| [is_text_wrapped](/cells/zh/python-net/aspose.cells.charts/legend/is_text_wrapped) |获取或设置一个值，该值指示文本是否换行。|
| [is_resize_shape_to_fit_text](/cells/zh/python-net/aspose.cells.charts/legend/is_resize_shape_to_fit_text) |获取或设置形状是否应自动调整以完全包含其中描述的文本。<br/>当缩放形状内的文本以包含内部的所有文本时。|
| [position](/cells/zh/python-net/aspose.cells.charts/legend/position) |获取或设置图例位置类型。|
| [legend_entries](/cells/zh/python-net/aspose.cells.charts/legend/legend_entries) |获取指定图表图例中所有 LegendEntry 对象的集合。<br/>不支持设置曲面图的图例项。<br/>因此，如果图表类型是曲面图表类型，它将返回 null。|
| [legend_entries_labels](/cells/zh/python-net/aspose.cells.charts/legend/legend_entries_labels) |调用 Chart.Calculate() 方法后获取图例条目的标签。|
| [is_over_lay](/cells/zh/python-net/aspose.cells.charts/legend/is_over_lay) |获取或设置是否允许其他图表元素与该图表元素重叠。|


### 方法
|方法|描述|
| :- | :- |
| [set_position_auto()](/cells/zh/python-net/aspose.cells.charts/legend/set_position_auto/#) |将框架的位置设置为自动|
| [characters(start_index, length)](/cells/zh/python-net/aspose.cells.charts/legend/characters/#int-int) |返回一个 Characters 对象，该对象表示文本中的一系列字符。|



### 例子

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType, LegendPositionType

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
# Set Legend's width and height
legend = chart.legend
# Legend is at right side of chart by default.
# If the legend is at left or right side of the chart, setting Legend.X property will not take effect.
# If the legend is at top or bottom side of the chart, setting Legend.Y property will not take effect.
legend.y = 1500
legend.width = 50
legend.height = 50
# Set legend's position
legend.position = LegendPositionType.LEFT

```

### 也可以看看
* 模块 [aspose.cells.charts](..)
* 类 [ChartFrame](/cells/zh/python-net/aspose.cells.charts/chartframe)
* 类 [ChartTextFrame](/cells/zh/python-net/aspose.cells.charts/charttextframe)
* 类 [Legend](/cells/zh/python-net/aspose.cells.charts/legend)
* 类 [Line](/cells/zh/python-net/aspose.cells.drawing/line)
