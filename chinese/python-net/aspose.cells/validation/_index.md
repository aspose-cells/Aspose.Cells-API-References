---
title: Validation类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 1540
url: /zh/python-net/aspose.cells/validation/
is_root: false
---
##  Validation类
代表数据validation.settings。



Validation 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [operator](/cells/zh/python-net/aspose.cells/validation/operator) |表示数据验证的运算符。|
| [alert_style](/cells/zh/python-net/aspose.cells/validation/alert_style) |表示验证警报样式。|
| [type](/cells/zh/python-net/aspose.cells/validation/type) |表示数据验证类型。|
| [input_message](/cells/zh/python-net/aspose.cells/validation/input_message) |表示数据验证输入消息。|
| [input_title](/cells/zh/python-net/aspose.cells/validation/input_title) |表示数据验证输入对话框的标题。|
| [error_message](/cells/zh/python-net/aspose.cells/validation/error_message) |表示数据验证错误消息。|
| [error_title](/cells/zh/python-net/aspose.cells/validation/error_title) |表示数据验证错误对话框的标题。|
| [show_input](/cells/zh/python-net/aspose.cells/validation/show_input) |指示是否在用户选择数据验证范围内的单元格时显示数据验证输入消息。|
| [show_error](/cells/zh/python-net/aspose.cells/validation/show_error) |指示是否在用户输入无效数据时显示数据验证错误消息。|
| [ignore_blank](/cells/zh/python-net/aspose.cells/validation/ignore_blank) |指示范围数据验证是否允许空白值。|
| [formula1](/cells/zh/python-net/aspose.cells/validation/formula1) |表示与数据验证关联的值或表达式。|
| [formula2](/cells/zh/python-net/aspose.cells/validation/formula2) |表示与数据验证关联的值或表达式。|
| [value1](/cells/zh/python-net/aspose.cells/validation/value1) |表示与数据验证关联的第一个值。|
| [value2](/cells/zh/python-net/aspose.cells/validation/value2) |表示与数据验证关联的第二个值。|
| [in_cell_drop_down](/cells/zh/python-net/aspose.cells/validation/in_cell_drop_down) |指示数据验证是否显示包含可接受值的下拉列表。|
| [areas](/cells/zh/python-net/aspose.cells/validation/areas) |获取所有包含数据验证设置的 [CellArea](/cells/zh/python-net/aspose.cells/cellarea)。|


### 方法
|方法|描述|
| :- | :- |
| [get_formula1(is_r1c1, is_local)](/cells/zh/python-net/aspose.cells/validation/get_formula1/#bool-bool) |获取与此验证关联的值或表达式。|
| [get_formula1(is_r1c1, is_local, row, column)](/cells/zh/python-net/aspose.cells/validation/get_formula1/#bool-bool-int-int) |获取与特定单元格的此验证关联的值或表达式。|
| [get_formula2(is_r1c1, is_local)](/cells/zh/python-net/aspose.cells/validation/get_formula2/#bool-bool) |获取与此验证关联的值或表达式。|
| [get_formula2(is_r1c1, is_local, row, column)](/cells/zh/python-net/aspose.cells/validation/get_formula2/#bool-bool-int-int) |获取与特定单元格的此验证关联的值或表达式。|
| [add_area(cell_area)](/cells/zh/python-net/aspose.cells/validation/add_area/#CellArea) |将验证应用于该区域。|
| [add_area(cell_area, check_intersection, check_edge)](/cells/zh/python-net/aspose.cells/validation/add_area/#CellArea-bool-bool) |将验证应用于该区域。|
| [set_formula1(formula, is_r1c1, is_local)](/cells/zh/python-net/aspose.cells/validation/set_formula1/#str-bool-bool) |设置与此验证关联的值或表达式。|
| [set_formula2(formula, is_r1c1, is_local)](/cells/zh/python-net/aspose.cells/validation/set_formula2/#str-bool-bool) |设置与此验证关联的值或表达式。|
| [get_list_value(row, column)](/cells/zh/python-net/aspose.cells/validation/get_list_value/#int-int) |获取指定单元格的验证列表的值。|
| [add_areas(areas, check_intersection, check_edge)](/cells/zh/python-net/aspose.cells/validation/add_areas/#list-bool-bool) |将验证应用于给定区域。|
| [remove_area(cell_area)](/cells/zh/python-net/aspose.cells/validation/remove_area/#CellArea) |删除范围内的验证设置。|
| [remove_areas(areas)](/cells/zh/python-net/aspose.cells/validation/remove_areas/#list) |从给定区域中删除此验证。|
| [remove_a_cell(row, column)](/cells/zh/python-net/aspose.cells/validation/remove_a_cell/#int-int) |删除单元格中的验证设置。|
| [copy(source, copy_option)](/cells/zh/python-net/aspose.cells/validation/copy/#Validation-CopyOptions) |复制验证。|



### 例子

```python
from aspose.cells import CellArea, OperatorType, ValidationType, Workbook

workbook = Workbook()
validations = workbook.worksheets[0].validations
area = CellArea.create_cell_area(0, 0, 1, 1)
validation = validations[validations.add(area)]
validation.type = ValidationType.WHOLE_NUMBER
validation.operator = OperatorType.BETWEEN
validation.formula1 = "3"
validation.formula2 = "1234"

```

### 也可以看看
* 模块 [aspose.cells](..)
* 类 [CellArea](/cells/zh/python-net/aspose.cells/cellarea)
