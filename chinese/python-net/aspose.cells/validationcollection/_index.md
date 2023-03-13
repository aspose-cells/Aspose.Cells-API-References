---
title: ValidationCollection类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 1550
url: /zh/python-net/aspose.cells/validationcollection/
is_root: false
---
## ValidationCollection类
表示数据验证集合。



ValidationCollection 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [capacity](/cells/zh/python-net/aspose.cells/validationcollection/capacity) |获取或设置数组列表可以包含的元素数。|


### 方法
|方法|描述|
| :- | :- |
| [add()](/cells/zh/python-net/aspose.cells/validationcollection/add/#) |向集合添加数据验证。|
| [add(ca)](/cells/zh/python-net/aspose.cells/validationcollection/add/#CellArea) |向集合添加数据验证。|
| [copy_to(array)](/cells/zh/python-net/aspose.cells/validationcollection/copy_to/#list) |将整个数组列表复制到兼容的一维数组列表，从目标数组列表的开头开始。|
| [copy_to(index, array, array_index, count)](/cells/zh/python-net/aspose.cells/validationcollection/copy_to/#int-list-int-int) |将数组列表中的一系列元素复制到兼容的一维数组列表，从目标数组列表的指定索引开始。|
| [index_of(item, index)](/cells/zh/python-net/aspose.cells/validationcollection/index_of/#Validation-int) |搜索指定的对象并返回数组列表中从指定索引延伸到最后一个元素的元素范围内第一次出现的从零开始的索引。|
| [index_of(item, index, count)](/cells/zh/python-net/aspose.cells/validationcollection/index_of/#Validation-int-int) |搜索指定的对象并返回数组列表中从指定索引开始并包含指定数量的元素的元素范围内第一次出现的从零开始的索引。|
| [last_index_of(item)](/cells/zh/python-net/aspose.cells/validationcollection/last_index_of/#Validation) |搜索指定的对象并返回整个数组列表中最后一次出现的从零开始的索引。|
| [last_index_of(item, index)](/cells/zh/python-net/aspose.cells/validationcollection/last_index_of/#Validation-int) |搜索指定的对象并返回数组列表中从第一个元素到指定索引的元素范围内最后一次出现的从零开始的索引。|
| [last_index_of(item, index, count)](/cells/zh/python-net/aspose.cells/validationcollection/last_index_of/#Validation-int-int) |搜索指定的对象并返回数组列表中包含指定数量的元素并以指定索引结束的元素范围内最后一次出现的从零开始的索引。|
| [remove_a_cell(row, column)](/cells/zh/python-net/aspose.cells/validationcollection/remove_a_cell/#int-int) |删除单元格上的所有验证设置。|
| [remove_area(ca)](/cells/zh/python-net/aspose.cells/validationcollection/remove_area/#CellArea) |删除范围内的所有验证设置..|
| [get_validation_in_cell(row, column)](/cells/zh/python-net/aspose.cells/validationcollection/get_validation_in_cell/#int-int) |获取应用于给定单元格的验证。|
| [binary_search(item)](/cells/zh/python-net/aspose.cells/validationcollection/binary_search/#Validation) |使用默认比较器在整个排序数组列表中搜索元素，并返回元素的从零开始的索引。|



### 例子

```python
from aspose.cells import CellArea, ValidationType, Workbook

workbook = Workbook()
validations = workbook.worksheets[0].validations
area = CellArea.create_cell_area(0, 0, 1, 1)
validation = validations[validations.add(area)]
validation.type = ValidationType.LIST
validation.formula1 = "a,b,c,d"

```

### 也可以看看
* 模块 [aspose.cells](..)
