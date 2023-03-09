---
title: CellWatchCollection类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 170
url: /zh/python-net/aspose.cells/cellwatchcollection/
is_root: false
---
## CellWatchCollection类
表示在“监视窗口”中监视的此工作表上的单元格集合。



CellWatchCollection 类型公开了以下成员：

### 构造器
|构造器|描述|
| :- | :- |
| [CellWatchCollection()](/cells/zh/python-net/aspose.cells/cellwatchcollection/__init__/#) |构造 CellWatchCollection 的新实例|


### 特性
|属性|描述|
| :- | :- |
| [capacity](/cells/zh/python-net/aspose.cells/cellwatchcollection/capacity) |获取或设置数组列表可以包含的元素数。|


### 方法
|方法|描述|
| :- | :- |
| [add(row, column)](/cells/zh/python-net/aspose.cells/cellwatchcollection/add/#int-int) |添加带有行和列的 [CellWatch](/cells/zh/python-net/aspose.cells/cellwatch)。|
| [add(cell_name)](/cells/zh/python-net/aspose.cells/cellwatchcollection/add/#str) |添加 [CellWatch](/cells/zh/python-net/aspose.cells/cellwatch) 和单元格的名称。|
| [copy_to(array)](/cells/zh/python-net/aspose.cells/cellwatchcollection/copy_to/#list) |将整个数组列表复制到兼容的一维数组列表，从目标数组列表的开头开始。|
| [copy_to(index, array, array_index, count)](/cells/zh/python-net/aspose.cells/cellwatchcollection/copy_to/#int-list-int-int) |将数组列表中的一系列元素复制到兼容的一维数组列表，从目标数组列表的指定索引开始。|
| [index_of(item, index)](/cells/zh/python-net/aspose.cells/cellwatchcollection/index_of/#CellWatch-int) |搜索指定的对象并返回数组列表中从指定索引延伸到最后一个元素的元素范围内第一次出现的从零开始的索引。|
| [index_of(item, index, count)](/cells/zh/python-net/aspose.cells/cellwatchcollection/index_of/#CellWatch-int-int) |搜索指定的对象并返回数组列表中从指定索引开始并包含指定数量的元素的元素范围内第一次出现的从零开始的索引。|
| [last_index_of(item)](/cells/zh/python-net/aspose.cells/cellwatchcollection/last_index_of/#CellWatch) |搜索指定的对象并返回整个数组列表中最后一次出现的从零开始的索引。|
| [last_index_of(item, index)](/cells/zh/python-net/aspose.cells/cellwatchcollection/last_index_of/#CellWatch-int) |搜索指定的对象并返回数组列表中从第一个元素到指定索引的元素范围内最后一次出现的从零开始的索引。|
| [last_index_of(item, index, count)](/cells/zh/python-net/aspose.cells/cellwatchcollection/last_index_of/#CellWatch-int-int) |搜索指定的对象并返回数组列表中包含指定数量的元素并以指定索引结束的元素范围内最后一次出现的从零开始的索引。|
| [binary_search(item)](/cells/zh/python-net/aspose.cells/cellwatchcollection/binary_search/#CellWatch) |使用默认比较器在整个排序数组列表中搜索元素，并返回元素的从零开始的索引。|



### 例子

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
#  Get the first Worksheet.
sheet = workbook.worksheets[0]
#  Add Cell Watch Item into the watch window
sheet.cell_watches.add("B2")

```

### 也可以看看
* 模块 [aspose.cells](..)
* 类 [CellWatch](/cells/zh/python-net/aspose.cells/cellwatch)
