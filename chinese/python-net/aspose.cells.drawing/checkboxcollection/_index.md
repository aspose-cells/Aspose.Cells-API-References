---
title: CheckBoxCollection类
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 100
url: /zh/python-net/aspose.cells.drawing/checkboxcollection/
is_root: false
---
## CheckBoxCollection类
表示工作表中 [CheckBox](/cells/zh/python-net/aspose.cells.drawing/checkbox) 对象的集合。



CheckBoxCollection 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [capacity](/cells/zh/python-net/aspose.cells.drawing/checkboxcollection/capacity) |获取或设置数组列表可以包含的元素数。|


### 方法
|方法|描述|
| :- | :- |
| [copy_to(array)](/cells/zh/python-net/aspose.cells.drawing/checkboxcollection/copy_to/#list) |将整个数组列表复制到兼容的一维数组列表，从目标数组列表的开头开始。|
| [copy_to(index, array, array_index, count)](/cells/zh/python-net/aspose.cells.drawing/checkboxcollection/copy_to/#int-list-int-int) |将数组列表中的一系列元素复制到兼容的一维数组列表，从目标数组列表的指定索引开始。|
| [index_of(item, index)](/cells/zh/python-net/aspose.cells.drawing/checkboxcollection/index_of/#CheckBox-int) |搜索指定的对象并返回数组列表中从指定索引延伸到最后一个元素的元素范围内第一次出现的从零开始的索引。|
| [index_of(item, index, count)](/cells/zh/python-net/aspose.cells.drawing/checkboxcollection/index_of/#CheckBox-int-int) |搜索指定的对象并返回数组列表中从指定索引开始并包含指定数量的元素的元素范围内第一次出现的从零开始的索引。|
| [last_index_of(item)](/cells/zh/python-net/aspose.cells.drawing/checkboxcollection/last_index_of/#CheckBox) |搜索指定的对象并返回整个数组列表中最后一次出现的从零开始的索引。|
| [last_index_of(item, index)](/cells/zh/python-net/aspose.cells.drawing/checkboxcollection/last_index_of/#CheckBox-int) |搜索指定的对象并返回数组列表中从第一个元素到指定索引的元素范围内最后一次出现的从零开始的索引。|
| [last_index_of(item, index, count)](/cells/zh/python-net/aspose.cells.drawing/checkboxcollection/last_index_of/#CheckBox-int-int) |搜索指定的对象并返回数组列表中包含指定数量的元素并以指定索引结束的元素范围内最后一次出现的从零开始的索引。|
| [add(upper_left_row, upper_left_column, height, width)](/cells/zh/python-net/aspose.cells.drawing/checkboxcollection/add/#int-int-int-int) |向集合中添加一个复选框。|
| [binary_search(item)](/cells/zh/python-net/aspose.cells.drawing/checkboxcollection/binary_search/#CheckBox) |使用默认比较器在整个排序数组列表中搜索元素，并返回元素的从零开始的索引。|



### 例子

```python
from aspose.cells import Workbook

# Create a new Workbook.
workbook = Workbook()
# Get the first worksheet in the workbook.
sheet = workbook.worksheets[0]
index = sheet.check_boxes.add(15, 15, 20, 100)
checkBox = sheet.check_boxes[index]
checkBox.text = "Check Box 1"

```

### 也可以看看
* 模块 [aspose.cells.drawing](..)
* 类 [CheckBox](/cells/zh/python-net/aspose.cells.drawing/checkbox)
