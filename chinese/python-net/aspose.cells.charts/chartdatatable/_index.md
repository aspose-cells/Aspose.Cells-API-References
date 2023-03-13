---
title: ChartDataTable类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 60
url: /zh/python-net/aspose.cells.charts/chartdatatable/
is_root: false
---
## ChartDataTable类
表示图表数据表。



ChartDataTable 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [font](/cells/zh/python-net/aspose.cells.charts/chartdatatable/font) |获取一个[ChartDataTable.font](/cells/zh/python-net/aspose.cells.charts/chartdatatable#font)对象，代表指定图表数据表的字体设置。|
| [auto_scale_font](/cells/zh/python-net/aspose.cells.charts/chartdatatable/auto_scale_font) |如果对象中的文本在对象大小更改时更改字体大小，则为真。<br/>默认值是true。|
| [background_mode](/cells/zh/python-net/aspose.cells.charts/chartdatatable/background_mode) |获取和设置背景的显示方式|
| [background](/cells/zh/python-net/aspose.cells.charts/chartdatatable/background) |获取和设置背景的显示方式|
| [has_border_horizontal](/cells/zh/python-net/aspose.cells.charts/chartdatatable/has_border_horizontal) |如果图表数据表具有水平单元格边框则为真|
| [has_border_vertical](/cells/zh/python-net/aspose.cells.charts/chartdatatable/has_border_vertical) |如果图表数据表具有垂直单元格边框则为真|
| [has_border_outline](/cells/zh/python-net/aspose.cells.charts/chartdatatable/has_border_outline) |如果图表数据表有轮廓边框则为真|
| [show_legend_key](/cells/zh/python-net/aspose.cells.charts/chartdatatable/show_legend_key) |如果数据标签图例键可见，则为真。|
| [border](/cells/zh/python-net/aspose.cells.charts/chartdatatable/border) |返回表示对象边框的 Border 对象|



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
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 25, 10)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.n_series.add("A1:B3", True)
chart.show_data_table = True
# Getting Chart Table
chartTable = chart.chart_data_table
# Setting Chart Table Font Color
chartTable.font.color = Color.red
# Setting Legend Key VisibilityOptions
chartTable.show_legend_key = False
# Saving the Excel file
workbook.save("book1.xls")

```

### 也可以看看
* 模块 [aspose.cells.charts](..)
