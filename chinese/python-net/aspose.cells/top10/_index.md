---
title: Top10类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 1480
url: /zh/python-net/aspose.cells/top10/
is_root: false
---
## Top10类
描述 Top10 条件格式规则。
此条件格式规则突出显示其单元格
值落在顶部 N 或底部 N 括号中，如指定的那样。



Top10 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [Top10()](/cells/zh/python-net/aspose.cells/top10/__init__/#) |构造 Top10 的新实例|


### 特性
|属性|描述|
| :- | :- |
| [is_percent](/cells/zh/python-net/aspose.cells/top10/is_percent) |获取或设置“top/bottom n”规则是否为“top/bottom n percent”规则。<br/>默认值为假。|
| [is_bottom](/cells/zh/python-net/aspose.cells/top10/is_bottom) |获取或设置“top/bottom n”规则是否为“bottom n”规则。<br/>默认值为假。|
| [rank](/cells/zh/python-net/aspose.cells/top10/rank) |获取或设置“top/bottom n”条件格式规则中“n”的值。<br/>如果 IsPercent 为真，则该值必须介于 0 和 100 之间。<br/>否则它必须介于 0 和 1000 之间。<br/>默认值为 10。|



### 例子

```python
from aspose.cells import CellArea, FormatConditionType, OperatorType, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea.create_cell_area(0, 0, 10, 10)
fcs.add_area(ca)
# Adds condition.
conditionIndex = fcs.add_condition(FormatConditionType.TOP10, OperatorType.NONE, None, None)
# Sets the background color.
fc = fcs[conditionIndex]
fc.style.background_color = Color.red
top10 = fc.top10
# Set the Top N
top10.rank = 5
# Saving the Excel file
workbook.save("output.xls")

```

### 也可以看看
* 模块 [aspose.cells](..)
