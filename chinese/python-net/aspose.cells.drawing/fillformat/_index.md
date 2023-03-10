---
title: FillFormat类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 180
url: /zh/python-net/aspose.cells.drawing/fillformat/
is_root: false
---
## FillFormat类
封装表示形状填充格式的对象。



FillFormat 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [type](/cells/zh/python-net/aspose.cells.drawing/fillformat/type) |获取和设置填充类型。|
| [fill_type](/cells/zh/python-net/aspose.cells.drawing/fillformat/fill_type) |获取和设置填充类型|
| [transparency](/cells/zh/python-net/aspose.cells.drawing/fillformat/transparency) |将区域的透明度返回或设置为从 0.0（不透明）到 1.0（透明）的值。|
| [set_type](/cells/zh/python-net/aspose.cells.drawing/fillformat/set_type) |获取填充格式集类型。|
| [gradient_fill](/cells/zh/python-net/aspose.cells.drawing/fillformat/gradient_fill) |获取 [FillFormat.gradient_fill](/cells/zh/python-net/aspose.cells.drawing/fillformat#gradient_fill) 对象。|
| [texture_fill](/cells/zh/python-net/aspose.cells.drawing/fillformat/texture_fill) |获取 [FillFormat.texture_fill](/cells/zh/python-net/aspose.cells.drawing/fillformat#texture_fill) 对象。|
| [solid_fill](/cells/zh/python-net/aspose.cells.drawing/fillformat/solid_fill) |获取 [FillFormat.solid_fill](/cells/zh/python-net/aspose.cells.drawing/fillformat#solid_fill) 对象。|
| [pattern_fill](/cells/zh/python-net/aspose.cells.drawing/fillformat/pattern_fill) |获取 [FillFormat.pattern_fill](/cells/zh/python-net/aspose.cells.drawing/fillformat#pattern_fill) 对象。|
| [gradient_color_type](/cells/zh/python-net/aspose.cells.drawing/fillformat/gradient_color_type) |返回指定填充的渐变颜色类型。|
| [gradient_style](/cells/zh/python-net/aspose.cells.drawing/fillformat/gradient_style) |返回指定填充的渐变样式。|
| [gradient_color1](/cells/zh/python-net/aspose.cells.drawing/fillformat/gradient_color1) |返回指定填充的渐变颜色 1。|
| [gradient_color2](/cells/zh/python-net/aspose.cells.drawing/fillformat/gradient_color2) |返回指定填充的渐变颜色 2。|
| [gradient_degree](/cells/zh/python-net/aspose.cells.drawing/fillformat/gradient_degree) |返回指定填充的渐变度。<br/>仅适用于 Excel 2007。|
| [gradient_variant](/cells/zh/python-net/aspose.cells.drawing/fillformat/gradient_variant) |返回指定填充的渐变变体。<br/>仅适用于 Excel 2007。|
| [preset_color](/cells/zh/python-net/aspose.cells.drawing/fillformat/preset_color) |返回指定填充的渐变预设颜色。|
| [texture](/cells/zh/python-net/aspose.cells.drawing/fillformat/texture) |表示指定填充的纹理类型。|
| [pattern](/cells/zh/python-net/aspose.cells.drawing/fillformat/pattern) |表示一个区域的显示模式。|
| [picture_format_type](/cells/zh/python-net/aspose.cells.drawing/fillformat/picture_format_type) |获取和设置图片格式类型。|
| [scale](/cells/zh/python-net/aspose.cells.drawing/fillformat/scale) |获取和设置图片格式比例。|
| [image_data](/cells/zh/python-net/aspose.cells.drawing/fillformat/image_data) |获取和设置图片图像数据。|


### 方法
|方法|描述|
| :- | :- |
| [set_two_color_gradient(color1, color2, style, variant)](/cells/zh/python-net/aspose.cells.drawing/fillformat/set_two_color_gradient/#aspose.pydrawing.Color-aspose.pydrawing.Color-GradientStyleType-int) |将指定的填充设置为双色渐变。<br/>仅适用于 Excel 2007。|
| [set_two_color_gradient(color1, transparency1, color2, transparency2, style, variant)](/cells/zh/python-net/aspose.cells.drawing/fillformat/set_two_color_gradient/#aspose.pydrawing.Color-float-aspose.pydrawing.Color-float-GradientStyleType-int) |将指定的填充设置为双色渐变。<br/>仅适用于 Excel 2007。|
| [set_one_color_gradient(color, degree, style, variant)](/cells/zh/python-net/aspose.cells.drawing/fillformat/set_one_color_gradient/#aspose.pydrawing.Color-float-GradientStyleType-int) |将指定的填充设置为单色渐变。<br/>仅适用于 Excel 2007。|
| [set_preset_color_gradient(preset_color, style, variant)](/cells/zh/python-net/aspose.cells.drawing/fillformat/set_preset_color_gradient/#GradientPresetType-GradientStyleType-int) |将指定的填充设置为预设颜色渐变。<br/>仅适用于 Excel 2007。|



### 例子

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType
from aspose.cells.drawing import GradientStyleType
from aspose.pydrawing import Color

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
seriesIndex = chart.n_series.add("A1:B4", True)
# Setting the data source for the category data of NSeries
chart.n_series.category_data = "C1:C4"
# Filling the area of the 2nd NSeries with a gradient
chart.n_series[seriesIndex].area.fill_format.set_one_color_gradient(Color.lime, 1, GradientStyleType.HORIZONTAL, 1)

```

### 也可以看看
* 模块 [aspose.cells.drawing](..)
