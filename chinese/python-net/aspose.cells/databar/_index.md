---
title: DataBar类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 400
url: /zh/python-net/aspose.cells/databar/
is_root: false
---
## DataBar类
描述 DataBar 条件格式规则。
此条件格式规则显示渐变
单元格区域中的数据栏。



DataBar 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [axis_color](/cells/zh/python-net/aspose.cells/databar/axis_color) |获取具有条件格式的单元格的轴颜色作为数据条。|
| [axis_position](/cells/zh/python-net/aspose.cells/databar/axis_position) |获取或设置由条件格式规则指定的数据条轴的位置。|
| [bar_fill_type](/cells/zh/python-net/aspose.cells/databar/bar_fill_type) |获取或设置数据条如何填充颜色。|
| [direction](/cells/zh/python-net/aspose.cells/databar/direction) |获取或设置数据栏的显示方向。|
| [bar_border](/cells/zh/python-net/aspose.cells/databar/bar_border) |获取一个对象，该对象指定数据栏的边框。|
| [negative_bar_format](/cells/zh/python-net/aspose.cells/databar/negative_bar_format) |获取与数据栏条件格式设置规则关联的 NegativeBarFormat 对象。|
| [min_cfvo](/cells/zh/python-net/aspose.cells/databar/min_cfvo) |获取或设置此 DataBar 的最小值对象。<br/>无法为其设置 null 或类型为 FormatConditionValueType.Max 的 CFValueObject。|
| [max_cfvo](/cells/zh/python-net/aspose.cells/databar/max_cfvo) |获取或设置此 DataBar 的最大值对象。<br/>无法为其设置 null 或类型为 FormatConditionValueType.Min 的 CFValueObject。|
| [color](/cells/zh/python-net/aspose.cells/databar/color) |获取或设置此 DataBar 的颜色。|
| [min_length](/cells/zh/python-net/aspose.cells/databar/min_length) |表示数据条的最小长度。|
| [max_length](/cells/zh/python-net/aspose.cells/databar/max_length) |表示数据条的最大长度。|
| [show_value](/cells/zh/python-net/aspose.cells/databar/show_value) |获取或设置标志，指示是否显示应用此数据栏的单元格的值。<br/>默认值为真。|


### 方法
|方法|描述|
| :- | :- |
| [to_image(cell, img_opts)](/cells/zh/python-net/aspose.cells/databar/to_image/#Cell-aspose.cells.rendering.ImageOrPrintOptions) |将单元格中的数据条渲染为图像字节数组。|



### 例子

```python
from aspose.cells import CellArea, DataBarAxisPosition, DataBarBorderType, DataBarFillType, DataBarNegativeColorType, FormatConditionType, FormatConditionValueType, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea()
ca.start_row = 0
ca.end_row = 2
ca.start_column = 0
ca.end_column = 0
fcs.add_area(ca)
# Adds condition.
idx = fcs.add_condition(FormatConditionType.DATA_BAR)
fcs.add_area(ca)
cond = fcs[idx]
# Get Databar
dataBar = cond.data_bar
dataBar.color = Color.orange
# Set Databar properties
dataBar.min_cfvo.type = FormatConditionValueType.PERCENTILE
dataBar.min_cfvo.value = 30
dataBar.show_value = False
dataBar.bar_border.type = DataBarBorderType.SOLID
dataBar.bar_border.color = Color.plum
dataBar.bar_fill_type = DataBarFillType.SOLID
dataBar.axis_color = Color.red
dataBar.axis_position = DataBarAxisPosition.MIDPOINT
dataBar.negative_bar_format.color_type = DataBarNegativeColorType.COLOR
dataBar.negative_bar_format.color = Color.white
dataBar.negative_bar_format.border_color_type = DataBarNegativeColorType.COLOR
dataBar.negative_bar_format.border_color = Color.yellow
# Put Cell Values
cell1 = sheet.cells.get("A1")
cell1.put_value(10)
cell2 = sheet.cells.get("A2")
cell2.put_value(120)
cell3 = sheet.cells.get("A3")
cell3.put_value(260)
# Saving the Excel file
workbook.save("book1.xlsx")

```

### 也可以看看
* 模块 [aspose.cells](..)
