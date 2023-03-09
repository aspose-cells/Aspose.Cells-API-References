---
title: HyperlinkCollection类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 800
url: /zh/python-net/aspose.cells/hyperlinkcollection/
is_root: false
---
## HyperlinkCollection类
封装 [Hyperlink](/cells/zh/python-net/aspose.cells/hyperlink) 对象的集合。



HyperlinkCollection 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [capacity](/cells/zh/python-net/aspose.cells/hyperlinkcollection/capacity) |获取或设置数组列表可以包含的元素数。|


### 方法
|方法|描述|
| :- | :- |
| [add(first_row, first_column, total_rows, total_columns, address)](/cells/zh/python-net/aspose.cells/hyperlinkcollection/add/#int-int-int-int-str) |添加指向指定单元格或单元格区域的超链接。|
| [add(cell_name, total_rows, total_columns, address)](/cells/zh/python-net/aspose.cells/hyperlinkcollection/add/#str-int-int-str) |添加指向指定单元格或单元格区域的超链接。|
| [add(start_cell_name, end_cell_name, address, text_to_display, screen_tip)](/cells/zh/python-net/aspose.cells/hyperlinkcollection/add/#str-str-str-str-str) |添加指向指定单元格或单元格区域的超链接。|
| [copy_to(array)](/cells/zh/python-net/aspose.cells/hyperlinkcollection/copy_to/#list) |将整个数组列表复制到兼容的一维数组列表，从目标数组列表的开头开始。|
| [copy_to(index, array, array_index, count)](/cells/zh/python-net/aspose.cells/hyperlinkcollection/copy_to/#int-list-int-int) |将数组列表中的一系列元素复制到兼容的一维数组列表，从目标数组列表的指定索引开始。|
| [index_of(item, index)](/cells/zh/python-net/aspose.cells/hyperlinkcollection/index_of/#Hyperlink-int) |搜索指定的对象并返回数组列表中从指定索引延伸到最后一个元素的元素范围内第一次出现的从零开始的索引。|
| [index_of(item, index, count)](/cells/zh/python-net/aspose.cells/hyperlinkcollection/index_of/#Hyperlink-int-int) |搜索指定的对象并返回数组列表中从指定索引开始并包含指定数量的元素的元素范围内第一次出现的从零开始的索引。|
| [last_index_of(item)](/cells/zh/python-net/aspose.cells/hyperlinkcollection/last_index_of/#Hyperlink) |搜索指定的对象并返回整个数组列表中最后一次出现的从零开始的索引。|
| [last_index_of(item, index)](/cells/zh/python-net/aspose.cells/hyperlinkcollection/last_index_of/#Hyperlink-int) |搜索指定的对象并返回数组列表中从第一个元素到指定索引的元素范围内最后一次出现的从零开始的索引。|
| [last_index_of(item, index, count)](/cells/zh/python-net/aspose.cells/hyperlinkcollection/last_index_of/#Hyperlink-int-int) |搜索指定的对象并返回数组列表中包含指定数量的元素并以指定索引结束的元素范围内最后一次出现的从零开始的索引。|
| [binary_search(item)](/cells/zh/python-net/aspose.cells/hyperlinkcollection/binary_search/#Hyperlink) |使用默认比较器在整个排序数组列表中搜索元素，并返回元素的从零开始的索引。|



### 例子

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[0]
# Get Hyperlinks Collection
hyperlinks = worksheet.hyperlinks
# Adding a hyperlink to a URL at "A1" cell
hyperlinks.add("A1", 1, 1, "http://www.aspose.com")
# Saving the Excel file
workbook.save("book1.xls")

```

### 也可以看看
* 模块 [aspose.cells](..)
* 类 [Hyperlink](/cells/zh/python-net/aspose.cells/hyperlink)
