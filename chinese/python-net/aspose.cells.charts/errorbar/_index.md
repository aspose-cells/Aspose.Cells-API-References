---
title: ErrorBar类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 150
url: /zh/python-net/aspose.cells.charts/errorbar/
is_root: false
---
## ErrorBar类
表示数据系列的误差线。



**继承：** [ErrorBar](/cells/python-net/aspose.cells.charts/errorbar) → 
[Line](/cells/zh/python-net/aspose.cells.drawing/line)



ErrorBar 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [compound_type](/cells/zh/python-net/aspose.cells.charts/errorbar/compound_type) |指定复合线型|
| [dash_type](/cells/zh/python-net/aspose.cells.charts/errorbar/dash_type) |指定虚线类型|
| [cap_type](/cells/zh/python-net/aspose.cells.charts/errorbar/cap_type) |指定结束大写。|
| [join_type](/cells/zh/python-net/aspose.cells.charts/errorbar/join_type) |指定连接帽。|
| [begin_type](/cells/zh/python-net/aspose.cells.charts/errorbar/begin_type) |指定行首的箭头。|
| [end_type](/cells/zh/python-net/aspose.cells.charts/errorbar/end_type) |指定行尾的箭头。|
| [begin_arrow_length](/cells/zh/python-net/aspose.cells.charts/errorbar/begin_arrow_length) |指定行首箭头的长度。|
| [end_arrow_length](/cells/zh/python-net/aspose.cells.charts/errorbar/end_arrow_length) |指定行尾箭头的长度。|
| [begin_arrow_width](/cells/zh/python-net/aspose.cells.charts/errorbar/begin_arrow_width) |指定行首箭头的宽度。|
| [end_arrow_width](/cells/zh/python-net/aspose.cells.charts/errorbar/end_arrow_width) |指定行尾箭头的宽度。|
| [theme_color](/cells/zh/python-net/aspose.cells.charts/errorbar/theme_color) |获取和设置主题颜色。|
| [color](/cells/zh/python-net/aspose.cells.charts/errorbar/color) |代表线的颜色。|
| [transparency](/cells/zh/python-net/aspose.cells.charts/errorbar/transparency) |将线条的透明度返回或设置为从 0.0（不透明）到 1.0（透明）的值。|
| [style](/cells/zh/python-net/aspose.cells.charts/errorbar/style) |表示线条的样式。|
| [weight](/cells/zh/python-net/aspose.cells.charts/errorbar/weight) |获取或设置线路的 [WeightType](/cells/zh/python-net/aspose.cells.drawing/weighttype)。|
| [weight_pt](/cells/zh/python-net/aspose.cells.charts/errorbar/weight_pt) |以点为单位获取或设置线的权重。|
| [weight_px](/cells/zh/python-net/aspose.cells.charts/errorbar/weight_px) |以像素为单位获取或设置线条的粗细。|
| [formatting_type](/cells/zh/python-net/aspose.cells.charts/errorbar/formatting_type) |获取或设置格式类型。|
| [is_automatic_color](/cells/zh/python-net/aspose.cells.charts/errorbar/is_automatic_color) |指示线的颜色是否自动分配。|
| [is_visible](/cells/zh/python-net/aspose.cells.charts/errorbar/is_visible) |表示线条是否可见。|
| [is_auto](/cells/zh/python-net/aspose.cells.charts/errorbar/is_auto) |指示此线型是否自动指定。|
| [gradient_fill](/cells/zh/python-net/aspose.cells.charts/errorbar/gradient_fill) |代表渐变填充。|
| [type](/cells/zh/python-net/aspose.cells.charts/errorbar/type) |表示错误栏金额类型。|
| [display_type](/cells/zh/python-net/aspose.cells.charts/errorbar/display_type) |表示错误栏显示类型。|
| [amount](/cells/zh/python-net/aspose.cells.charts/errorbar/amount) |表示误差条的数量。<br/>金额必须大于或等于零。|
| [show_marker_t_top](/cells/zh/python-net/aspose.cells.charts/errorbar/show_marker_t_top) |指示是否使用 T 形顶部格式化错误栏。|
| [plus_value](/cells/zh/python-net/aspose.cells.charts/errorbar/plus_value) |当错误栏类型为自定义时，表示正错误量。|
| [minus_value](/cells/zh/python-net/aspose.cells.charts/errorbar/minus_value) |当错误栏类型为自定义时，表示负错误量。|



### 例子

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType, ErrorBarDisplayType, ErrorBarType

workbook = Workbook()
cells = workbook.worksheets[0].cells
cells.get("a1").put_value(2)
cells.get("a2").put_value(5)
cells.get("a3").put_value(3)
cells.get("a4").put_value(6)
cells.get("b1").put_value(4)
cells.get("b2").put_value(3)
cells.get("b3").put_value(6)
cells.get("b4").put_value(7)
cells.get("C1").put_value("Q1")
cells.get("C2").put_value("Q2")
cells.get("C3").put_value("Y1")
cells.get("C4").put_value("Y2")
chartIndex = workbook.worksheets[0].charts.add(ChartType.COLUMN, 11, 0, 27, 10)
chart = workbook.worksheets[0].charts[chartIndex]
chart.n_series.add("A1:B4", True)
chart.n_series.category_data = "C1:C4"
for i in range(len(chart.NSeries)):
    aseries = chart.n_series[i]
    aseries.y_error_bar.display_type = ErrorBarDisplayType.MINUS
    aseries.y_error_bar.type = ErrorBarType.FIXED_VALUE
    aseries.y_error_bar.amount = 5

```

### 也可以看看
* 模块 [aspose.cells.charts](..)
* 类 [ErrorBar](/cells/zh/python-net/aspose.cells.charts/errorbar)
* 类 [Line](/cells/zh/python-net/aspose.cells.drawing/line)
* 类 [WeightType](/cells/zh/python-net/aspose.cells.drawing/weighttype)
