---
title: Trendline类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 330
url: /zh/python-net/aspose.cells.charts/trendline/
is_root: false
---
##  Trendline类
代表图表中的趋势线。



**继承：** [Trendline](/cells/python-net/aspose.cells.charts/trendline) → 
[Line](/cells/zh/python-net/aspose.cells.drawing/line)



Trendline 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [compound_type](/cells/zh/python-net/aspose.cells.charts/trendline/compound_type) |指定复合线型|
| [dash_type](/cells/zh/python-net/aspose.cells.charts/trendline/dash_type) |指定虚线类型|
| [cap_type](/cells/zh/python-net/aspose.cells.charts/trendline/cap_type) |指定结束大写。|
| [join_type](/cells/zh/python-net/aspose.cells.charts/trendline/join_type) |指定连接帽。|
| [begin_type](/cells/zh/python-net/aspose.cells.charts/trendline/begin_type) |指定行首的箭头。|
| [end_type](/cells/zh/python-net/aspose.cells.charts/trendline/end_type) |指定行尾的箭头。|
| [begin_arrow_length](/cells/zh/python-net/aspose.cells.charts/trendline/begin_arrow_length) |指定行首箭头的长度。|
| [end_arrow_length](/cells/zh/python-net/aspose.cells.charts/trendline/end_arrow_length) |指定行尾箭头的长度。|
| [begin_arrow_width](/cells/zh/python-net/aspose.cells.charts/trendline/begin_arrow_width) |指定行首箭头的宽度。|
| [end_arrow_width](/cells/zh/python-net/aspose.cells.charts/trendline/end_arrow_width) |指定行尾箭头的宽度。|
| [theme_color](/cells/zh/python-net/aspose.cells.charts/trendline/theme_color) |获取和设置主题颜色。|
| [color](/cells/zh/python-net/aspose.cells.charts/trendline/color) |代表线的颜色。|
| [transparency](/cells/zh/python-net/aspose.cells.charts/trendline/transparency) |将线条的透明度返回或设置为从 0.0（不透明）到 1.0（透明）的值。|
| [style](/cells/zh/python-net/aspose.cells.charts/trendline/style) |表示线条的样式。|
| [weight](/cells/zh/python-net/aspose.cells.charts/trendline/weight) |获取或设置线路的 [WeightType](/cells/zh/python-net/aspose.cells.drawing/weighttype)。|
| [weight_pt](/cells/zh/python-net/aspose.cells.charts/trendline/weight_pt) |以点为单位获取或设置线的权重。|
| [weight_px](/cells/zh/python-net/aspose.cells.charts/trendline/weight_px) |以像素为单位获取或设置线条的粗细。|
| [formatting_type](/cells/zh/python-net/aspose.cells.charts/trendline/formatting_type) |获取或设置格式类型。|
| [is_automatic_color](/cells/zh/python-net/aspose.cells.charts/trendline/is_automatic_color) |指示线的颜色是否自动分配。|
| [is_visible](/cells/zh/python-net/aspose.cells.charts/trendline/is_visible) |表示线条是否可见。|
| [is_auto](/cells/zh/python-net/aspose.cells.charts/trendline/is_auto) |指示此线型是否自动指定。|
| [gradient_fill](/cells/zh/python-net/aspose.cells.charts/trendline/gradient_fill) |代表渐变填充。|
| [is_name_auto](/cells/zh/python-net/aspose.cells.charts/trendline/is_name_auto) |返回 if Microsoft Excel 自动确定趋势线的名称。|
| [type](/cells/zh/python-net/aspose.cells.charts/trendline/type) |返回趋势线类型。|
| [name](/cells/zh/python-net/aspose.cells.charts/trendline/name) |返回趋势线的名称。|
| [order](/cells/zh/python-net/aspose.cells.charts/trendline/order) |当趋势线类型为 Polynomial 时，返回或设置趋势线顺序（大于 1 的整数）。<br/>顺序必须在 2 到 6 之间。|
| [period](/cells/zh/python-net/aspose.cells.charts/trendline/period) |返回或设置移动平均趋势线的周期。|
| [forward](/cells/zh/python-net/aspose.cells.charts/trendline/forward) |返回或设置趋势线向前延伸的周期数（或散点图上的单位）。<br/>周期数必须大于或等于零。|
| [backward](/cells/zh/python-net/aspose.cells.charts/trendline/backward) |返回或设置趋势线向后延伸的周期数（或散点图上的单位）。<br/>周期数必须大于或等于零。<br/>如果图表类型为柱状图，周期数必须在 0 到 0.5 之间|
| [display_equation](/cells/zh/python-net/aspose.cells.charts/trendline/display_equation) |表示趋势线的方程式是否显示在图表上（在与 R 平方值相同的数据标签中）。将此属性设置为 True 会自动打开数据标签。|
| [display_r_squared](/cells/zh/python-net/aspose.cells.charts/trendline/display_r_squared) |表示趋势线的 R 平方值是否显示在图表上（在与方程式相同的数据标签中）。将此属性设置为 True 会自动打开数据标签。|
| [intercept](/cells/zh/python-net/aspose.cells.charts/trendline/intercept) |返回或设置趋势线穿过数值轴的点。|
| [data_labels](/cells/zh/python-net/aspose.cells.charts/trendline/data_labels) |表示指定系列的 DataLabels 对象。|
| [legend_entry](/cells/zh/python-net/aspose.cells.charts/trendline/legend_entry) |根据这条趋势线获取图例条目|



### 例子

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType, TrendlineType

# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Excel object
sheetIndex = workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[sheetIndex]
# Adding a sample value to "A1" cell
worksheet.cells.get("A1").put_value(50)
# Adding a sample value to "A2" cell
worksheet.cells.get("A2").put_value(100)
# Adding a sample value to "A3" cell
worksheet.cells.get("A3").put_value(150)
# Adding a sample value to "A4" cell
worksheet.cells.get("A4").put_value(200)
# Adding a sample value to "B1" cell
worksheet.cells.get("B1").put_value(60)
# Adding a sample value to "B2" cell
worksheet.cells.get("B2").put_value(32)
# Adding a sample value to "B3" cell
worksheet.cells.get("B3").put_value(50)
# Adding a sample value to "B4" cell
worksheet.cells.get("B4").put_value(40)
# Adding a sample value to "C1" cell as category data
worksheet.cells.get("C1").put_value("Q1")
# Adding a sample value to "C2" cell as category data
worksheet.cells.get("C2").put_value("Q2")
# Adding a sample value to "C3" cell as category data
worksheet.cells.get("C3").put_value("Y1")
# Adding a sample value to "C4" cell as category data
worksheet.cells.get("C4").put_value("Y2")
# Adding a chart to the worksheet
chartIndex = worksheet.charts.add(ChartType.COLUMN, 5, 0, 15, 5)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B4"
chart.n_series.add("A1:B4", True)
# Setting the data source for the category data of NSeries
chart.n_series.category_data = "C1:C4"
# adding a linear trendline
index = chart.n_series[0].trend_lines.add(TrendlineType.LINEAR)
trendline = chart.n_series[0].trend_lines[index]
# Setting the custom name of the trendline.
trendline.name = "Linear"
# Displaying the equation on chart
trendline.display_equation = True
# Displaying the R-Squared value on chart
trendline.display_r_squared = True
# Saving the Excel file
workbook.save("book1.xls")

```

### 也可以看看
* 模块 [aspose.cells.charts](..)
* 类 [Line](/cells/zh/python-net/aspose.cells.drawing/line)
* 类 [Trendline](/cells/zh/python-net/aspose.cells.charts/trendline)
* 类 [WeightType](/cells/zh/python-net/aspose.cells.drawing/weighttype)
