---
title: HorizontalPageBreakCollection类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 760
url: /zh/python-net/aspose.cells/horizontalpagebreakcollection/
is_root: false
---
##  HorizontalPageBreakCollection类
封装 [HorizontalPageBreak](/cells/zh/python-net/aspose.cells/horizontalpagebreak) 对象的集合。



HorizontalPageBreakCollection 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [capacity](/cells/zh/python-net/aspose.cells/horizontalpagebreakcollection/capacity) |获取或设置数组列表可以包含的元素数。|


### 方法
|方法|描述|
| :- | :- |
| [add(row, start_column, end_column)](/cells/zh/python-net/aspose.cells/horizontalpagebreakcollection/add/#int-int-int) |向集合中添加水平分页符。|
| [add(row)](/cells/zh/python-net/aspose.cells/horizontalpagebreakcollection/add/#int) |向集合中添加水平分页符。|
| [add(row, column)](/cells/zh/python-net/aspose.cells/horizontalpagebreakcollection/add/#int-int) |向集合中添加水平分页符。|
| [add(cell_name)](/cells/zh/python-net/aspose.cells/horizontalpagebreakcollection/add/#str) |向集合中添加水平分页符。|
| [copy_to(array)](/cells/zh/python-net/aspose.cells/horizontalpagebreakcollection/copy_to/#list) |将整个数组列表复制到兼容的一维数组列表，从目标数组列表的开头开始。|
| [copy_to(index, array, array_index, count)](/cells/zh/python-net/aspose.cells/horizontalpagebreakcollection/copy_to/#int-list-int-int) |将数组列表中的一系列元素复制到兼容的一维数组列表，从目标数组列表的指定索引开始。|
| [index_of(item, index)](/cells/zh/python-net/aspose.cells/horizontalpagebreakcollection/index_of/#HorizontalPageBreak-int) |搜索指定的对象并返回数组列表中从指定索引延伸到最后一个元素的元素范围内第一次出现的从零开始的索引。|
| [index_of(item, index, count)](/cells/zh/python-net/aspose.cells/horizontalpagebreakcollection/index_of/#HorizontalPageBreak-int-int) |搜索指定的对象并返回数组列表中从指定索引开始并包含指定数量的元素的元素范围内第一次出现的从零开始的索引。|
| [last_index_of(item)](/cells/zh/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak) |搜索指定的对象并返回整个数组列表中最后一次出现的从零开始的索引。|
| [last_index_of(item, index)](/cells/zh/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak-int) |搜索指定的对象并返回数组列表中从第一个元素到指定索引的元素范围内最后一次出现的从零开始的索引。|
| [last_index_of(item, index, count)](/cells/zh/python-net/aspose.cells/horizontalpagebreakcollection/last_index_of/#HorizontalPageBreak-int-int) |搜索指定的对象并返回数组列表中包含指定数量的元素并以指定索引结束的元素范围内最后一次出现的从零开始的索引。|
| [binary_search(item)](/cells/zh/python-net/aspose.cells/horizontalpagebreakcollection/binary_search/#HorizontalPageBreak) |使用默认比较器在整个排序数组列表中搜索元素，并返回元素的从零开始的索引。|



### 例子

```python
from aspose.cells import Workbook

excel = Workbook()
# Add a pagebreak at G5
excel.worksheets[0].horizontal_page_breaks.add("G5")
excel.worksheets[0].vertical_page_breaks.add("G5")

```

### 也可以看看
* 模块 [aspose.cells](..)
* 类 [HorizontalPageBreak](/cells/zh/python-net/aspose.cells/horizontalpagebreak)
