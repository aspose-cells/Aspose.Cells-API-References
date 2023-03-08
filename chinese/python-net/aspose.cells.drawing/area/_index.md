---
title: Area类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells.drawing/area/
is_root: false
---
##  Area类
封装表示区域格式的对象。



Area 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [background_color](/cells/zh/python-net/aspose.cells.drawing/area/background_color) |获取或设置 [Area](/cells/zh/python-net/aspose.cells.drawing/area) 的背景颜色。|
| [foreground_color](/cells/zh/python-net/aspose.cells.drawing/area/foreground_color) |获取或设置前景颜色。|
| [formatting](/cells/zh/python-net/aspose.cells.drawing/area/formatting) |表示区域的格式。|
| [invert_if_negative](/cells/zh/python-net/aspose.cells.drawing/area/invert_if_negative) |如果该属性为真且图表点的值为负数，<br/>前景色和背景色将交换。|
| [fill_format](/cells/zh/python-net/aspose.cells.drawing/area/fill_format) |表示包含指定图表或形状的填充格式属性的 [Area.fill_format](/cells/zh/python-net/aspose.cells.drawing/area#fill_format) 对象。|
| [transparency](/cells/zh/python-net/aspose.cells.drawing/area/transparency) |将区域的透明度返回或设置为从 0.0（不透明）到 1.0（透明）的值。|



### 例子

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Workbook object
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
# Setting the foreground color of the plot area
chart.plot_area.area.foreground_color = Color.blue
# Setting the foreground color of the chart area
chart.chart_area.area.foreground_color = Color.yellow
# Setting the foreground color of the 1st NSeries area
chart.n_series[0].area.foreground_color = Color.red
# Setting the foreground color of the area of the 1st NSeries point
chart.n_series[0].points[0].area.foreground_color = Color.cyan
# Saving the Excel file
workbook.save("book1.xls")

```

### 也可以看看
* 模块 [aspose.cells.drawing](..)
* 类 [Area](/cells/zh/python-net/aspose.cells.drawing/area)
