---
title: PictureCollection类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 460
url: /zh/python-net/aspose.cells.drawing/picturecollection/
is_root: false
---
##  PictureCollection类
封装 [Picture](/cells/zh/python-net/aspose.cells.drawing/picture) 对象的集合。



PictureCollection 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [capacity](/cells/zh/python-net/aspose.cells.drawing/picturecollection/capacity) |获取或设置数组列表可以包含的元素数。|


### 方法
|方法|描述|
| :- | :- |
| [add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream)](/cells/zh/python-net/aspose.cells.drawing/picturecollection/add/#int-int-int-int-io.RawIOBase) |将图片添加到集合中。|
| [add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name)](/cells/zh/python-net/aspose.cells.drawing/picturecollection/add/#int-int-int-int-str) |将图片添加到集合中。|
| [add(upper_left_row, upper_left_column, stream)](/cells/zh/python-net/aspose.cells.drawing/picturecollection/add/#int-int-io.RawIOBase) |将图片添加到集合中。|
| [add(upper_left_row, upper_left_column, file_name)](/cells/zh/python-net/aspose.cells.drawing/picturecollection/add/#int-int-str) |将图片添加到集合中。|
| [add(upper_left_row, upper_left_column, stream, width_scale, height_scale)](/cells/zh/python-net/aspose.cells.drawing/picturecollection/add/#int-int-io.RawIOBase-int-int) |将图片添加到集合中。|
| [add(upper_left_row, upper_left_column, file_name, width_scale, height_scale)](/cells/zh/python-net/aspose.cells.drawing/picturecollection/add/#int-int-str-int-int) |将图片添加到集合中。|
| [copy_to(array)](/cells/zh/python-net/aspose.cells.drawing/picturecollection/copy_to/#list) |将整个数组列表复制到兼容的一维数组列表，从目标数组列表的开头开始。|
| [copy_to(index, array, array_index, count)](/cells/zh/python-net/aspose.cells.drawing/picturecollection/copy_to/#int-list-int-int) |将数组列表中的一系列元素复制到兼容的一维数组列表，从目标数组列表的指定索引开始。|
| [index_of(item, index)](/cells/zh/python-net/aspose.cells.drawing/picturecollection/index_of/#Picture-int) |搜索指定的对象并返回数组列表中从指定索引延伸到最后一个元素的元素范围内第一次出现的从零开始的索引。|
| [index_of(item, index, count)](/cells/zh/python-net/aspose.cells.drawing/picturecollection/index_of/#Picture-int-int) |搜索指定的对象并返回数组列表中从指定索引开始并包含指定数量的元素的元素范围内第一次出现的从零开始的索引。|
| [last_index_of(item)](/cells/zh/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture) |搜索指定的对象并返回整个数组列表中最后一次出现的从零开始的索引。|
| [last_index_of(item, index)](/cells/zh/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture-int) |搜索指定的对象并返回数组列表中从第一个元素到指定索引的元素范围内最后一次出现的从零开始的索引。|
| [last_index_of(item, index, count)](/cells/zh/python-net/aspose.cells.drawing/picturecollection/last_index_of/#Picture-int-int) |搜索指定的对象并返回数组列表中包含指定数量的元素并以指定索引结束的元素范围内最后一次出现的从零开始的索引。|
| [binary_search(item)](/cells/zh/python-net/aspose.cells.drawing/picturecollection/binary_search/#Picture) |使用默认比较器在整个排序数组列表中搜索元素，并返回元素的从零开始的索引。|



### 例子

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# get PictureCollection
pictures = workbook.worksheets[0].pictures
# do your business
# Save the excel file.
workbook.save("result.xlsx")

```

### 也可以看看
* 模块 [aspose.cells.drawing](..)
* 类 [Picture](/cells/zh/python-net/aspose.cells.drawing/picture)
