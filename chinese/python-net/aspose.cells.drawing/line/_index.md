---
title: Line类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 290
url: /zh/python-net/aspose.cells.drawing/line/
is_root: false
---
##  Line类
封装表示行格式的对象。



Line 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [compound_type](/cells/zh/python-net/aspose.cells.drawing/line/compound_type) |指定复合线型|
| [dash_type](/cells/zh/python-net/aspose.cells.drawing/line/dash_type) |指定虚线类型|
| [cap_type](/cells/zh/python-net/aspose.cells.drawing/line/cap_type) |指定结束大写。|
| [join_type](/cells/zh/python-net/aspose.cells.drawing/line/join_type) |指定连接帽。|
| [begin_type](/cells/zh/python-net/aspose.cells.drawing/line/begin_type) |指定行首的箭头。|
| [end_type](/cells/zh/python-net/aspose.cells.drawing/line/end_type) |指定行尾的箭头。|
| [begin_arrow_length](/cells/zh/python-net/aspose.cells.drawing/line/begin_arrow_length) |指定行首箭头的长度。|
| [end_arrow_length](/cells/zh/python-net/aspose.cells.drawing/line/end_arrow_length) |指定行尾箭头的长度。|
| [begin_arrow_width](/cells/zh/python-net/aspose.cells.drawing/line/begin_arrow_width) |指定行首箭头的宽度。|
| [end_arrow_width](/cells/zh/python-net/aspose.cells.drawing/line/end_arrow_width) |指定行尾箭头的宽度。|
| [theme_color](/cells/zh/python-net/aspose.cells.drawing/line/theme_color) |获取和设置主题颜色。|
| [color](/cells/zh/python-net/aspose.cells.drawing/line/color) |代表线的颜色。|
| [transparency](/cells/zh/python-net/aspose.cells.drawing/line/transparency) |将线条的透明度返回或设置为从 0.0（不透明）到 1.0（透明）的值。|
| [style](/cells/zh/python-net/aspose.cells.drawing/line/style) |表示线条的样式。|
| [weight](/cells/zh/python-net/aspose.cells.drawing/line/weight) |获取或设置线路的 [WeightType](/cells/zh/python-net/aspose.cells.drawing/weighttype)。|
| [weight_pt](/cells/zh/python-net/aspose.cells.drawing/line/weight_pt) |以点为单位获取或设置线的权重。|
| [weight_px](/cells/zh/python-net/aspose.cells.drawing/line/weight_px) |以像素为单位获取或设置线条的粗细。|
| [formatting_type](/cells/zh/python-net/aspose.cells.drawing/line/formatting_type) |获取或设置格式类型。|
| [is_automatic_color](/cells/zh/python-net/aspose.cells.drawing/line/is_automatic_color) |指示线的颜色是否自动分配。|
| [is_visible](/cells/zh/python-net/aspose.cells.drawing/line/is_visible) |表示线条是否可见。|
| [is_auto](/cells/zh/python-net/aspose.cells.drawing/line/is_auto) |指示此线型是否自动指定。|
| [gradient_fill](/cells/zh/python-net/aspose.cells.drawing/line/gradient_fill) |代表渐变填充。|



### 例子

```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartMarkerType, ChartType
from aspose.cells.drawing import LineType, WeightType
from aspose.pydrawing import Color

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
chartIndex = sheet.charts.add(ChartType.LINE, 9, 9, 21, 15)
chart = sheet.charts[chartIndex]
# Applying a dotted line style on the lines of an NSeries
chart.n_series[0].border.style = LineType.DOT
chart.n_series[0].border.color = Color.red
# Applying a triangular marker style on the data markers of an NSeries
chart.n_series[0].marker.marker_style = ChartMarkerType.TRIANGLE
# Setting the weight of all lines in an NSeries to medium
chart.n_series[0].border.weight = WeightType.MEDIUM_LINE

```

### 也可以看看
* 模块 [aspose.cells.drawing](..)
* 类 [WeightType](/cells/zh/python-net/aspose.cells.drawing/weighttype)
