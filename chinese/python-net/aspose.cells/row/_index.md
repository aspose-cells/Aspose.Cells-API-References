---
title: Row类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 1300
url: /zh/python-net/aspose.cells/row/
is_root: false
---
## Row类
代表工作表中的一行。



Row 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [is_blank](/cells/zh/python-net/aspose.cells/row/is_blank) |指示该行是否包含任何数据|
| [is_collapsed](/cells/zh/python-net/aspose.cells/row/is_collapsed) |行是否折叠|
| [height](/cells/zh/python-net/aspose.cells/row/height) |获取和设置以 Points 为单位的行高。|
| [is_hidden](/cells/zh/python-net/aspose.cells/row/is_hidden) |指示行是否隐藏。|
| [index](/cells/zh/python-net/aspose.cells/row/index) |获取该行的索引。|
| [group_level](/cells/zh/python-net/aspose.cells/row/group_level) |获取行的组级别。|
| [is_height_matched](/cells/zh/python-net/aspose.cells/row/is_height_matched) |指示行高和默认字体高度匹配。|
| [style](/cells/zh/python-net/aspose.cells/row/style) |表示该行的样式。|
| [has_custom_style](/cells/zh/python-net/aspose.cells/row/has_custom_style) |指示此行是否具有自定义样式设置（不同于从工作簿继承的默认样式设置）。|
| [first_cell](/cells/zh/python-net/aspose.cells/row/first_cell) |获取行中的第一个单元格对象。|
| [first_data_cell](/cells/zh/python-net/aspose.cells/row/first_data_cell) |获取行中的第一个非空白单元格。|
| [last_cell](/cells/zh/python-net/aspose.cells/row/last_cell) |获取行中的最后一个单元格对象。|
| [last_data_cell](/cells/zh/python-net/aspose.cells/row/last_data_cell) |获取行中的最后一个非空白单元格。|



获取单元格。
### 索引器
|名称|描述|
| :- | :- |
| [index] |列索引|


### 方法
|方法|描述|
| :- | :- |
| [get_cell_by_index(index)](/cells/zh/python-net/aspose.cells/row/get_cell_by_index/#int) |通过列表中的特定索引获取单元格。|
| [get_cell_or_null(column)](/cells/zh/python-net/aspose.cells/row/get_cell_or_null/#int) |获取特定索引中的单元格或空值。|
| [get_style()](/cells/zh/python-net/aspose.cells/row/get_style/#) |获取此行的样式。|
| [set_style(style)](/cells/zh/python-net/aspose.cells/row/set_style/#Style) |设置此行的样式。|
| [copy_settings(source, check_style)](/cells/zh/python-net/aspose.cells/row/copy_settings/#Row-bool) |复制行的设置，例如样式、高度、可见性等。|
| [apply_style(style, flag)](/cells/zh/python-net/aspose.cells/row/apply_style/#Style-StyleFlag) |为整行应用格式。|
| [equals(row)](/cells/zh/python-net/aspose.cells/row/equals/#Row) |检查此对象是否引用与另一个行对象相同的行。|



### 例子

```python
from aspose.cells import BackgroundType, StyleFlag, Workbook
from aspose.pydrawing import Color

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
style = workbook.create_style()
# Setting the background color to Blue
style.background_color = Color.blue
# Setting the foreground color to Red
style.foreground_color = Color.red
# setting Background Pattern
style.pattern = BackgroundType.DIAGONAL_STRIPE
# New Style Flag
styleFlag = StyleFlag()
# Set All Styles
styleFlag.all = True
# Get first row
row = worksheet.cells.rows[0]
# Apply Style to first row
row.apply_style(style, styleFlag)
# Saving the Excel file
workbook.save("book1.xls")

```

### 也可以看看
* 模块 [aspose.cells](..)
