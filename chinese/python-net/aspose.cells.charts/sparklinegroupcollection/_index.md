---
title: SparklineGroupCollection类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 290
url: /zh/python-net/aspose.cells.charts/sparklinegroupcollection/
is_root: false
---
##  SparklineGroupCollection类
封装 [SparklineGroup](/cells/zh/python-net/aspose.cells.charts/sparklinegroup) 对象的集合。



SparklineGroupCollection 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [capacity](/cells/zh/python-net/aspose.cells.charts/sparklinegroupcollection/capacity) |获取或设置数组列表可以包含的元素数。|


### 方法
|方法|描述|
| :- | :- |
| [copy_to(array)](/cells/zh/python-net/aspose.cells.charts/sparklinegroupcollection/copy_to/#list) |将整个数组列表复制到兼容的一维数组列表，从目标数组列表的开头开始。|
| [copy_to(index, array, array_index, count)](/cells/zh/python-net/aspose.cells.charts/sparklinegroupcollection/copy_to/#int-list-int-int) |将数组列表中的一系列元素复制到兼容的一维数组列表，从目标数组列表的指定索引开始。|
| [index_of(item, index)](/cells/zh/python-net/aspose.cells.charts/sparklinegroupcollection/index_of/#SparklineGroup-int) |搜索指定的对象并返回数组列表中从指定索引延伸到最后一个元素的元素范围内第一次出现的从零开始的索引。|
| [index_of(item, index, count)](/cells/zh/python-net/aspose.cells.charts/sparklinegroupcollection/index_of/#SparklineGroup-int-int) |搜索指定的对象并返回数组列表中从指定索引开始并包含指定数量的元素的元素范围内第一次出现的从零开始的索引。|
| [last_index_of(item)](/cells/zh/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#SparklineGroup) |搜索指定的对象并返回整个数组列表中最后一次出现的从零开始的索引。|
| [last_index_of(item, index)](/cells/zh/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#SparklineGroup-int) |搜索指定的对象并返回数组列表中从第一个元素到指定索引的元素范围内最后一次出现的从零开始的索引。|
| [last_index_of(item, index, count)](/cells/zh/python-net/aspose.cells.charts/sparklinegroupcollection/last_index_of/#SparklineGroup-int-int) |搜索指定的对象并返回数组列表中包含指定数量的元素并以指定索引结束的元素范围内最后一次出现的从零开始的索引。|
| [add(type, data_range, is_vertical, location_range)](/cells/zh/python-net/aspose.cells.charts/sparklinegroupcollection/add/#SparklineType-str-bool-CellArea) |将 [SparklineGroup](/cells/zh/python-net/aspose.cells.charts/sparklinegroup) 项目添加到集合中。|
| [clear_sparklines(cell_area)](/cells/zh/python-net/aspose.cells.charts/sparklinegroupcollection/clear_sparklines/#CellArea) |清除单元格区域内的迷你图。|
| [clear_sparkline_groups(cell_area)](/cells/zh/python-net/aspose.cells.charts/sparklinegroupcollection/clear_sparkline_groups/#CellArea) |清除与单元格区域重叠的迷你图组。|
| [binary_search(item)](/cells/zh/python-net/aspose.cells.charts/sparklinegroupcollection/binary_search/#SparklineGroup) |使用默认比较器在整个排序数组列表中搜索元素，并返回元素的从零开始的索引。|



### 例子

```python
from aspose.cells import CellArea, SaveFormat, Workbook
from aspose.cells.charts import SparklineType

book = Workbook()
sheet = book.worksheets[0]
sheet.cells.get("A1").put_value(5)
sheet.cells.get("B1").put_value(2)
sheet.cells.get("C1").put_value(1)
sheet.cells.get("D1").put_value(3)
#  Define the CellArea
ca = CellArea()
ca.start_column = 4
ca.end_column = 4
ca.start_row = 0
ca.end_row = 0
idx = sheet.sparkline_group_collection.add(SparklineType.LINE, "A1:D1", False, ca)
group = sheet.sparkline_group_collection[idx]
group.sparkline_collection.add(sheet.name + "!A1:D1", 0, 4)
book.save("output.xlsx", SaveFormat.XLSX)

```

### 也可以看看
* 模块 [aspose.cells.charts](..)
* 类 [SparklineGroup](/cells/zh/python-net/aspose.cells.charts/sparklinegroup)
