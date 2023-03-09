---
title: FormatConditionCollection类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 700
url: /zh/python-net/aspose.cells/formatconditioncollection/
is_root: false
---
## FormatConditionCollection类
表示条件格式。
FormatConditions 最多可以包含三种条件格式。



FormatConditionCollection 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [count](/cells/zh/python-net/aspose.cells/formatconditioncollection/count) |获取条件的计数。|
| [range_count](/cells/zh/python-net/aspose.cells/formatconditioncollection/range_count) |获取条件格式范围的计数。|



通过索引获取格式化条件。
### 索引器
|名称|描述|
| :- | :- |
| [index] |要返回的格式化条件的索引。|


### 方法
|方法|描述|
| :- | :- |
| [add_condition(type, operator_type, formula1, formula2)](/cells/zh/python-net/aspose.cells/formatconditioncollection/add_condition/#FormatConditionType-OperatorType-str-str) |添加格式化条件。|
| [add_condition(type)](/cells/zh/python-net/aspose.cells/formatconditioncollection/add_condition/#FormatConditionType) |添加格式条件。|
| [remove_area(index)](/cells/zh/python-net/aspose.cells/formatconditioncollection/remove_area/#int) |按索引删除条件格式的单元格范围。|
| [remove_area(start_row, start_column, total_rows, total_columns)](/cells/zh/python-net/aspose.cells/formatconditioncollection/remove_area/#int-int-int-int) |删除范围内的条件格式。|
| [add(cell_area, type, operator_type, formula1, formula2)](/cells/zh/python-net/aspose.cells/formatconditioncollection/add/#CellArea-FormatConditionType-OperatorType-str-str) |将格式化条件和受影响的单元格范围添加到 FormatConditions<br/>FormatConditions 最多可以包含三种条件格式。<br/>条件格式的公式中不允许引用其他工作表。|
| [add_area(cell_area)](/cells/zh/python-net/aspose.cells/formatconditioncollection/add_area/#CellArea) |添加条件格式的单元格范围。|
| [get_cell_area(index)](/cells/zh/python-net/aspose.cells/formatconditioncollection/get_cell_area/#int) |按索引获取条件格式的单元格范围。|
| [remove_condition(index)](/cells/zh/python-net/aspose.cells/formatconditioncollection/remove_condition/#int) |按索引删除格式化条件。|



### 例子

```python
from aspose.cells import CellArea, FormatConditionType, OperatorType, Workbook
from aspose.pydrawing import Color

# Create a new Workbook.
workbook = Workbook()
# Get the first worksheet.
sheet = workbook.worksheets[0]
# Adds an empty conditional formatting
index = sheet.conditional_formattings.add()
fcs = sheet.conditional_formattings[index]
# Sets the conditional format range.
ca = CellArea()
ca.start_row = 0
ca.end_row = 0
ca.start_column = 0
ca.end_column = 0
fcs.add_area(ca)
ca = CellArea()
ca.start_row = 1
ca.end_row = 1
ca.start_column = 1
ca.end_column = 1
fcs.add_area(ca)
# Adds condition.
conditionIndex = fcs.add_condition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100")
# Adds condition.
conditionIndex2 = fcs.add_condition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100")
# Sets the background color.
fc = fcs[conditionIndex]
fc.style.background_color = Color.red
# Saving the Excel file
workbook.save("output.xls")

```

### 也可以看看
* 模块 [aspose.cells](..)
