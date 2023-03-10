---
title: Range类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 1250
url: /zh/python-net/aspose.cells/range/
is_root: false
---
## Range类
封装表示电子表格中一系列单元格的对象。



Range 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [current_region](/cells/zh/python-net/aspose.cells/range/current_region) |返回代表当前区域的 Range 对象。<br/>当前区域是由空白行和空白列的任意组合界定的范围。|
| [hyperlinks](/cells/zh/python-net/aspose.cells/range/hyperlinks) |获取范围内的所有超链接。|
| [row_count](/cells/zh/python-net/aspose.cells/range/row_count) |获取范围内的行数。|
| [column_count](/cells/zh/python-net/aspose.cells/range/column_count) |获取范围内的列数。|
| [cell_count](/cells/zh/python-net/aspose.cells/range/cell_count) |获取范围内的所有单元格计数。|
| [name](/cells/zh/python-net/aspose.cells/range/name) |获取或设置范围的名称。|
| [refers_to](/cells/zh/python-net/aspose.cells/range/refers_to) |获取范围的引用。|
| [address](/cells/zh/python-net/aspose.cells/range/address) |获取范围地址。|
| [left](/cells/zh/python-net/aspose.cells/range/left) |获取从 A 列左边缘到范围左边缘的距离（以磅为单位）。|
| [top](/cells/zh/python-net/aspose.cells/range/top) |获取从第 1 行的上边缘到范围的上边缘的距离（以磅为单位）。|
| [width](/cells/zh/python-net/aspose.cells/range/width) |获取范围的宽度（以磅为单位）。|
| [height](/cells/zh/python-net/aspose.cells/range/height) |获取范围的宽度（以磅为单位）。|
| [first_row](/cells/zh/python-net/aspose.cells/range/first_row) |获取范围第一行的索引。|
| [first_column](/cells/zh/python-net/aspose.cells/range/first_column) |获取范围第一列的索引。|
| [value](/cells/zh/python-net/aspose.cells/range/value) |获取和设置范围的值。|
| [column_width](/cells/zh/python-net/aspose.cells/range/column_width) |设置或获取该范围的列宽|
| [row_height](/cells/zh/python-net/aspose.cells/range/row_height) |设置或获取此范围内行的高度|
| [entire_column](/cells/zh/python-net/aspose.cells/range/entire_column) |获取一个 Range 对象，该对象表示包含指定范围的整个一列（或多列）。|
| [entire_row](/cells/zh/python-net/aspose.cells/range/entire_row) |获取一个 Range 对象，该对象表示包含指定范围的整行（或多行）。|
| [worksheet](/cells/zh/python-net/aspose.cells/range/worksheet) |获取包含此范围的 [Range.worksheet](/cells/zh/python-net/aspose.cells/range#worksheet) 对象。|


### 方法
|方法|描述|
| :- | :- |
| [auto_fill(target)](/cells/zh/python-net/aspose.cells/range/auto_fill/#Range) |自动填充目标范围。|
| [auto_fill(target, auto_fill_type)](/cells/zh/python-net/aspose.cells/range/auto_fill/#Range-AutoFillType) |自动填充目标范围。|
| [set_style(style, explicit_flag)](/cells/zh/python-net/aspose.cells/range/set_style/#Style-bool) |应用单元格样式。|
| [set_style(style)](/cells/zh/python-net/aspose.cells/range/set_style/#Style) |设置范围的样式。|
| [set_outline_borders(border_style, border_color)](/cells/zh/python-net/aspose.cells/range/set_outline_borders/#CellBorderType-CellsColor) |在具有相同边框样式和颜色的一系列单元格周围设置轮廓边框。|
| [set_outline_borders(border_style, border_color)](/cells/zh/python-net/aspose.cells/range/set_outline_borders/#CellBorderType-aspose.pydrawing.Color) |在具有相同边框样式和颜色的一系列单元格周围设置轮廓边框。|
| [set_outline_borders(border_styles, border_colors)](/cells/zh/python-net/aspose.cells/range/set_outline_borders/#list-aspose.pydrawing.Color[]) |在一系列单元格周围设置线条边框。|
| [set_outline_border(border_edge, border_style, border_color)](/cells/zh/python-net/aspose.cells/range/set_outline_border/#BorderType-CellBorderType-CellsColor) |围绕一系列单元格设置轮廓边框。|
| [set_outline_border(border_edge, border_style, border_color)](/cells/zh/python-net/aspose.cells/range/set_outline_border/#BorderType-CellBorderType-aspose.pydrawing.Color) |围绕一系列单元格设置轮廓边框。|
| [copy(range, options)](/cells/zh/python-net/aspose.cells/range/copy/#Range-PasteOptions) |使用粘贴特殊选项复制范围。|
| [copy(range)](/cells/zh/python-net/aspose.cells/range/copy/#Range) |从源范围复制数据（包括公式）、格式、绘图对象等。|
| [get_enumerator()](/cells/zh/python-net/aspose.cells/range/get_enumerator/#) |获取此 Range 中单元格的枚举器。|
| [is_intersect(range)](/cells/zh/python-net/aspose.cells/range/is_intersect/#Range) |指示范围是否相交。|
| [intersect(range)](/cells/zh/python-net/aspose.cells/range/intersect/#Range) |返回一个 [Range](/cells/zh/python-net/aspose.cells/range) 对象，表示两个范围的矩形交集。|
| [union(range)](/cells/zh/python-net/aspose.cells/range/union/#Range) |返回两个范围的并集。|
| [merge()](/cells/zh/python-net/aspose.cells/range/merge/#) |将一系列单元格组合成一个单元格。|
| [un_merge()](/cells/zh/python-net/aspose.cells/range/un_merge/#) |取消合并此范围内的合并单元格。|
| [put_value(string_value, is_converted, set_style)](/cells/zh/python-net/aspose.cells/range/put_value/#str-bool-bool) |将一个值放入范围内，如果合适，该值将被转换为其他数据类型，并且单元格的数字格式将被重置。|
| [apply_style(style, flag)](/cells/zh/python-net/aspose.cells/range/apply_style/#Style-StyleFlag) |应用整个范围的格式。|
| [set_inside_borders(border_edge, line_style, border_color)](/cells/zh/python-net/aspose.cells/range/set_inside_borders/#BorderType-CellBorderType-CellsColor) |设置范围的内部边界。|
| [move_to(dest_row, dest_column)](/cells/zh/python-net/aspose.cells/range/move_to/#int-int) |将当前范围移动到目标范围。|
| [copy_data(range)](/cells/zh/python-net/aspose.cells/range/copy_data/#Range) |从源区域复制单元格数据（包括公式）。|
| [copy_value(range)](/cells/zh/python-net/aspose.cells/range/copy_value/#Range) |从源区域复制单元格值。|
| [copy_style(range)](/cells/zh/python-net/aspose.cells/range/copy_style/#Range) |从源范围复制样式设置。|
| [get_cell_or_null(row_offset, column_offset)](/cells/zh/python-net/aspose.cells/range/get_cell_or_null/#int-int) |获取此范围内的 [Cell](/cells/zh/python-net/aspose.cells/cell) 对象或 null。|
| [get_offset(row_offset, column_offset)](/cells/zh/python-net/aspose.cells/range/get_offset/#int-int) |通过偏移获取 [Range](/cells/zh/python-net/aspose.cells/range) 范围。|



### 例子

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet Cells.
cells = workbook.worksheets[0].cells
#  Create a range (A1:D3).
range = cells.create_range("A1", "D3")
#  Set value to the range.
range.value = "Hello"
# Save the Excel file
workbook.save("book1.xlsm")

```

### 也可以看看
* 模块 [aspose.cells](..)
* 类 [Cell](/cells/zh/python-net/aspose.cells/cell)
* 类 [Range](/cells/zh/python-net/aspose.cells/range)
