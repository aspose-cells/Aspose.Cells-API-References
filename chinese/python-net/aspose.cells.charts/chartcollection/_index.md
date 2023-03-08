---
title: ChartCollection类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 50
url: /zh/python-net/aspose.cells.charts/chartcollection/
is_root: false
---
##  ChartCollection类
封装 [Chart](/cells/zh/python-net/aspose.cells.charts/chart) 对象的集合。



ChartCollection 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [capacity](/cells/zh/python-net/aspose.cells.charts/chartcollection/capacity) |获取或设置数组列表可以包含的元素数。|


### 方法
|方法|描述|
| :- | :- |
| [add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column)](/cells/zh/python-net/aspose.cells.charts/chartcollection/add/#ChartType-int-int-int-int) |向集合中添加图表。|
| [add(type, data_range, top_row, left_column, right_row, bottom_column)](/cells/zh/python-net/aspose.cells.charts/chartcollection/add/#ChartType-str-int-int-int-int) |向集合中添加图表。|
| [add(data, data_range, is_vertical, top_row, left_column, right_row, bottom_column)](/cells/zh/python-net/aspose.cells.charts/chartcollection/add/#bytes-str-bool-int-int-int-int) |添加带有预设模板的图表。|
| [add(type, data_range, is_vertical, top_row, left_column, right_row, bottom_column)](/cells/zh/python-net/aspose.cells.charts/chartcollection/add/#ChartType-str-bool-int-int-int-int) |向集合中添加图表。|
| [get(index)](/cells/zh/python-net/aspose.cells.charts/chartcollection/get/#int) |添加 API for Python Via .Net.since this[int index] is unsupported|
| [get(name)](/cells/zh/python-net/aspose.cells.charts/chartcollection/get/#str) |添加 API for Python 通过 .Net.since this[string Chart] 不受支持|
| [copy_to(array)](/cells/zh/python-net/aspose.cells.charts/chartcollection/copy_to/#list) |将整个数组列表复制到兼容的一维数组列表，从目标数组列表的开头开始。|
| [copy_to(index, array, array_index, count)](/cells/zh/python-net/aspose.cells.charts/chartcollection/copy_to/#int-list-int-int) |将数组列表中的一系列元素复制到兼容的一维数组列表，从目标数组列表的指定索引开始。|
| [index_of(item, index)](/cells/zh/python-net/aspose.cells.charts/chartcollection/index_of/#Chart-int) |搜索指定的对象并返回数组列表中从指定索引延伸到最后一个元素的元素范围内第一次出现的从零开始的索引。|
| [index_of(item, index, count)](/cells/zh/python-net/aspose.cells.charts/chartcollection/index_of/#Chart-int-int) |搜索指定的对象并返回数组列表中从指定索引开始并包含指定数量的元素的元素范围内第一次出现的从零开始的索引。|
| [last_index_of(item)](/cells/zh/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart) |搜索指定的对象并返回整个数组列表中最后一次出现的从零开始的索引。|
| [last_index_of(item, index)](/cells/zh/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart-int) |搜索指定的对象并返回数组列表中从第一个元素到指定索引的元素范围内最后一次出现的从零开始的索引。|
| [last_index_of(item, index, count)](/cells/zh/python-net/aspose.cells.charts/chartcollection/last_index_of/#Chart-int-int) |搜索指定的对象并返回数组列表中包含指定数量的元素并以指定索引结束的元素范围内最后一次出现的从零开始的索引。|
| [add_floating_chart(type, left, top, width, height)](/cells/zh/python-net/aspose.cells.charts/chartcollection/add_floating_chart/#ChartType-int-int-int-int) |向集合中添加图表。|
| [binary_search(item)](/cells/zh/python-net/aspose.cells.charts/chartcollection/binary_search/#Chart) |使用默认比较器在整个排序数组列表中搜索元素，并返回元素的从零开始的索引。|



### 例子

```python
from aspose.cells import Workbook

workbook = Workbook()
charts = workbook.worksheets[0].charts

```

### 也可以看看
* 模块 [aspose.cells.charts](..)
* 类 [Chart](/cells/zh/python-net/aspose.cells.charts/chart)
