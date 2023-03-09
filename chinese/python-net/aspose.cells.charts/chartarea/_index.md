---
title: ChartArea类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 40
url: /zh/python-net/aspose.cells.charts/chartarea/
is_root: false
---
## ChartArea类
封装代表工作表中图表区域的对象。



**继承：** [ChartArea](/cells/python-net/aspose.cells.charts/chartarea) → 
[ChartFrame](/cells/zh/python-net/aspose.cells.charts/chartframe)



ChartArea 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [is_inner_mode](/cells/zh/python-net/aspose.cells.charts/chartarea/is_inner_mode) |指示绘图区域大小是否包括刻度线和轴标签。<br/> False 指定大小应确定绘图区域、刻度线和轴标签的大小。|
| [border](/cells/zh/python-net/aspose.cells.charts/chartarea/border) |获取 [Line](/cells/zh/python-net/aspose.cells.drawing/line)。|
| [area](/cells/zh/python-net/aspose.cells.charts/chartarea/area) |获取 [ChartFrame.area](/cells/zh/python-net/aspose.cells.charts/chartframe#area)。|
| [text_font](/cells/zh/python-net/aspose.cells.charts/chartarea/text_font) |获取指定 ChartFrame 对象的 [ChartFrame.font](/cells/zh/python-net/aspose.cells.charts/chartframe#font) 对象。|
| [text_options](/cells/zh/python-net/aspose.cells.charts/chartarea/text_options) |获取和设置文本的选项。|
| [font](/cells/zh/python-net/aspose.cells.charts/chartarea/font) |获取指定图表区域对象的 [ChartArea.font](/cells/zh/python-net/aspose.cells.charts/chartarea#font) 对象。|
| [auto_scale_font](/cells/zh/python-net/aspose.cells.charts/chartarea/auto_scale_font) |如果对象中的文本在对象大小更改时更改字体大小，则为真。|
| [background_mode](/cells/zh/python-net/aspose.cells.charts/chartarea/background_mode) |获取和设置背景的显示方式|
| [background](/cells/zh/python-net/aspose.cells.charts/chartarea/background) |获取和设置背景的显示方式|
| [is_automatic_size](/cells/zh/python-net/aspose.cells.charts/chartarea/is_automatic_size) |指示图表框是否自动调整大小。|
| [x](/cells/zh/python-net/aspose.cells.charts/chartarea/x) |获取或获取其左上角列的水平偏移量。|
| [y](/cells/zh/python-net/aspose.cells.charts/chartarea/y) |获取或获取其左上角行的垂直偏移量。|
| [height](/cells/zh/python-net/aspose.cells.charts/chartarea/height) |获取或设置与其右下角行的垂直偏移量。|
| [width](/cells/zh/python-net/aspose.cells.charts/chartarea/width) |获取或设置与其右下角列的水平偏移量。|
| [shadow](/cells/zh/python-net/aspose.cells.charts/chartarea/shadow) |如果框架有阴影，则为真。|
| [shape_properties](/cells/zh/python-net/aspose.cells.charts/chartarea/shape_properties) |获取 [ChartFrame.shape_properties](/cells/zh/python-net/aspose.cells.charts/chartframe#shape_properties) 对象。|
| [is_default_pos_be_set](/cells/zh/python-net/aspose.cells.charts/chartarea/is_default_pos_be_set) |指示是否设置了默认位置（DefaultX、DefaultY、DefaultWidth 和 DefaultHeight）。|
| [default_x](/cells/zh/python-net/aspose.cells.charts/chartarea/default_x) |表示默认位置的x|
| [default_y](/cells/zh/python-net/aspose.cells.charts/chartarea/default_y) |代表默认位置的y|
| [default_width](/cells/zh/python-net/aspose.cells.charts/chartarea/default_width) |表示默认位置的宽度|
| [default_height](/cells/zh/python-net/aspose.cells.charts/chartarea/default_height) |表示默认位置的高度|


### 方法
|方法|描述|
| :- | :- |
| [set_position_auto()](/cells/zh/python-net/aspose.cells.charts/chartarea/set_position_auto/#) |将框架的位置设置为自动|



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
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 15, 5)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.n_series.add("A1:B3", True)
# Getting Chart Area
chartArea = chart.chart_area
# Setting the foreground color of the chart area
chartArea.area.foreground_color = Color.yellow
# Setting Chart Area Shadow
chartArea.shadow = True
# Saving the Excel file
workbook.save("book1.xls")

```

### 也可以看看
* 模块 [aspose.cells.charts](..)
* 类 [ChartArea](/cells/zh/python-net/aspose.cells.charts/chartarea)
* 类 [ChartFrame](/cells/zh/python-net/aspose.cells.charts/chartframe)
* 类 [Line](/cells/zh/python-net/aspose.cells.drawing/line)
