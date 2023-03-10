---
title: VbaModuleCollection类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells.vba/vbamodulecollection/
is_root: false
---
## VbaModuleCollection类
代表列表[VbaModule](/cells/zh/python-net/aspose.cells.vba/vbamodule)



VbaModuleCollection 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [capacity](/cells/zh/python-net/aspose.cells.vba/vbamodulecollection/capacity) |获取或设置数组列表可以包含的元素数。|


### 方法
|方法|描述|
| :- | :- |
| [add(sheet)](/cells/zh/python-net/aspose.cells.vba/vbamodulecollection/add/#Worksheet) |为工作表添加模块。|
| [add(type, name)](/cells/zh/python-net/aspose.cells.vba/vbamodulecollection/add/#VbaModuleType-str) |添加模块。|
| [copy_to(array)](/cells/zh/python-net/aspose.cells.vba/vbamodulecollection/copy_to/#list) |将整个数组列表复制到兼容的一维数组列表，从目标数组列表的开头开始。|
| [copy_to(index, array, array_index, count)](/cells/zh/python-net/aspose.cells.vba/vbamodulecollection/copy_to/#int-list-int-int) |将数组列表中的一系列元素复制到兼容的一维数组列表，从目标数组列表的指定索引开始。|
| [index_of(item, index)](/cells/zh/python-net/aspose.cells.vba/vbamodulecollection/index_of/#VbaModule-int) |搜索指定的对象并返回数组列表中从指定索引延伸到最后一个元素的元素范围内第一次出现的从零开始的索引。|
| [index_of(item, index, count)](/cells/zh/python-net/aspose.cells.vba/vbamodulecollection/index_of/#VbaModule-int-int) |搜索指定的对象并返回数组列表中从指定索引开始并包含指定数量的元素的元素范围内第一次出现的从零开始的索引。|
| [last_index_of(item)](/cells/zh/python-net/aspose.cells.vba/vbamodulecollection/last_index_of/#VbaModule) |搜索指定的对象并返回整个数组列表中最后一次出现的从零开始的索引。|
| [last_index_of(item, index)](/cells/zh/python-net/aspose.cells.vba/vbamodulecollection/last_index_of/#VbaModule-int) |搜索指定的对象并返回数组列表中从第一个元素到指定索引的元素范围内最后一次出现的从零开始的索引。|
| [last_index_of(item, index, count)](/cells/zh/python-net/aspose.cells.vba/vbamodulecollection/last_index_of/#VbaModule-int-int) |搜索指定的对象并返回数组列表中包含指定数量的元素并以指定索引结束的元素范围内最后一次出现的从零开始的索引。|
| [add_designer_storage(name, data)](/cells/zh/python-net/aspose.cells.vba/vbamodulecollection/add_designer_storage/#str-bytes) |  |
| [get_designer_storage(name)](/cells/zh/python-net/aspose.cells.vba/vbamodulecollection/get_designer_storage/#str) |代表Designer的数据。|
| [binary_search(item)](/cells/zh/python-net/aspose.cells.vba/vbamodulecollection/binary_search/#VbaModule) |使用默认比较器在整个排序数组列表中搜索元素，并返回元素的从零开始的索引。|



### 例子

```python
from aspose.cells import Workbook
from aspose.cells.vba import VbaModuleType

# Instantiating a Workbook object
workbook = Workbook()
#  Init VBA project.
vbaProject = workbook.vba_project
#  Add a new module.
vbaProject.modules.add(VbaModuleType.CLASS, "test")
# Saving the Excel file
workbook.save("book1.xlsm")

```

### 也可以看看
* 模块 [aspose.cells.vba](..)
* 类 [VbaModule](/cells/zh/python-net/aspose.cells.vba/vbamodule)
