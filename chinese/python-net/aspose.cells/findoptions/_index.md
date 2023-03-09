---
title: FindOptions类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 630
url: /zh/python-net/aspose.cells/findoptions/
is_root: false
---
## FindOptions类
表示查找选项。



FindOptions 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [FindOptions()](/cells/zh/python-net/aspose.cells/findoptions/__init__/#) |构造 FindOptions 的新实例|


### 特性
|属性|描述|
| :- | :- |
| [is_case_sensitive](/cells/zh/python-net/aspose.cells/findoptions/is_case_sensitive) |指示搜索的字符串是否区分大小写。|
| [case_sensitive](/cells/zh/python-net/aspose.cells/findoptions/case_sensitive) |指示搜索的字符串是否区分大小写。|
| [look_at_type](/cells/zh/python-net/aspose.cells/findoptions/look_at_type) |看类型。|
| [is_range_set](/cells/zh/python-net/aspose.cells/findoptions/is_range_set) |表示是否设置了搜索范围。|
| [search_next](/cells/zh/python-net/aspose.cells/findoptions/search_next) |搜索顺序。True：搜索下一个。False：搜索上一个。|
| [search_backward](/cells/zh/python-net/aspose.cells/findoptions/search_backward) |是否向后搜索单元格。|
| [seach_order_by_rows](/cells/zh/python-net/aspose.cells/findoptions/seach_order_by_rows) |指示搜索顺序是按行还是按列。|
| [look_in_type](/cells/zh/python-net/aspose.cells/findoptions/look_in_type) |看类型。|
| [regex_key](/cells/zh/python-net/aspose.cells/findoptions/regex_key) |指示搜索的键是否为正则表达式。<br/>如果为真，则搜索到的键将被视为正则表达式并进行解析。|
| [value_type_sensitive](/cells/zh/python-net/aspose.cells/findoptions/value_type_sensitive) |指示搜索的单元格值类型是否应与搜索的键相同。|
| [style](/cells/zh/python-net/aspose.cells/findoptions/style) |要搜索的格式。|
| [convert_numeric_data](/cells/zh/python-net/aspose.cells/findoptions/convert_numeric_data) |获取或设置一个值，该值指示是否将搜索到的字符串值转换为数字数据。|


### 方法
|方法|描述|
| :- | :- |
| [get_range()](/cells/zh/python-net/aspose.cells/findoptions/get_range/#) |获取和设置搜索范围。|
| [set_range(ca)](/cells/zh/python-net/aspose.cells/findoptions/set_range/#CellArea) |设置搜索范围。|



### 例子

```python
from aspose.cells import CellArea, FindOptions, LookInType, Workbook

# Instantiate the workbook object
workbook = Workbook("book1.xls")
# Get Cells collection
cells = workbook.worksheets[0].cells
# Instantiate FindOptions Object
findOptions = FindOptions()
# Create a Cells Area
ca = CellArea()
ca.start_row = 8
ca.start_column = 2
ca.end_row = 17
ca.end_column = 13
# Set cells area for find options
findOptions.set_range(ca)
# Set searching properties
findOptions.search_backward = False
findOptions.seach_order_by_rows = True
findOptions.look_in_type = LookInType.VALUES
# Find the cell with 0 value
cell = cells.find(0, None, findOptions)

```

### 也可以看看
* 模块 [aspose.cells](..)
