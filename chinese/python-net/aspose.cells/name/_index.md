---
title: Name类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 1070
url: /zh/python-net/aspose.cells/name/
is_root: false
---
##  Name类
代表一系列单元格的定义名称。



Name 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [comment](/cells/zh/python-net/aspose.cells/name/comment) |获取和设置名称的注释。<br/>仅适用于 Excel 2007。|
| [text](/cells/zh/python-net/aspose.cells/name/text) |获取对象的名称文本。|
| [full_text](/cells/zh/python-net/aspose.cells/name/full_text) |获取具有范围设置的对象的名称全文。|
| [refers_to](/cells/zh/python-net/aspose.cells/name/refers_to) |返回或设置名称定义为引用的公式，以等号开头。|
| [r1c1_refers_to](/cells/zh/python-net/aspose.cells/name/r1c1_refers_to) |获取或设置 [Name](/cells/zh/python-net/aspose.cells/name) 的 R1C1 引用。|
| [is_referred](/cells/zh/python-net/aspose.cells/name/is_referred) |指示此名称是否被其他公式引用。|
| [is_visible](/cells/zh/python-net/aspose.cells/name/is_visible) |指示名称是否可见。|
| [sheet_index](/cells/zh/python-net/aspose.cells/name/sheet_index) |指示此名称属于工作簿或工作表。<br/> 0 = 全局名称，否则索引到工作表（从一开始）|


### 方法
|方法|描述|
| :- | :- |
| [get_refers_to(is_r1c1, is_local)](/cells/zh/python-net/aspose.cells/name/get_refers_to/#bool-bool) |获取此名称的引用。|
| [get_refers_to(is_r1c1, is_local, row, column)](/cells/zh/python-net/aspose.cells/name/get_refers_to/#bool-bool-int-int) |根据指定的单元格获取此名称的引用。|
| [get_ranges()](/cells/zh/python-net/aspose.cells/name/get_ranges/#) |获取由此名称引用的所有范围。|
| [get_ranges(recalculate)](/cells/zh/python-net/aspose.cells/name/get_ranges/#bool) |获取由此名称引用的所有范围。|
| [get_range()](/cells/zh/python-net/aspose.cells/name/get_range/#) |如果此名称引用范围，则获取范围。|
| [get_range(recalculate)](/cells/zh/python-net/aspose.cells/name/get_range/#bool) |如果此名称引用范围，则获取范围|
| [get_range(sheet_index, row, column)](/cells/zh/python-net/aspose.cells/name/get_range/#int-int-int) |如果此名称引用范围，则获取范围。<br/>如果此名称的引用不是绝对的，则不同单元格的范围可能不同。|
| [set_refers_to(refers_to, is_r1c1, is_local)](/cells/zh/python-net/aspose.cells/name/set_refers_to/#str-bool-bool) |设置此名称的引用。|
| [get_referred_areas(recalculate)](/cells/zh/python-net/aspose.cells/name/get_referred_areas/#bool) |获取由此名称引用的所有引用。|



### 例子

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Accessing the first worksheet in the Excel file
worksheet = workbook.worksheets[0]
# Creating a named range
range = worksheet.cells.create_range("B4", "G14")
# Setting the name of the named range
range.name = "TestRange"
# Saving the modified Excel file in default (that is Excel 2000) format
workbook.save("output.xls")

```

### 也可以看看
* 模块 [aspose.cells](..)
* 类 [Name](/cells/zh/python-net/aspose.cells/name)
