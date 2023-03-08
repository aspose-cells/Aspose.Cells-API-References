---
title: RowCollection类
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 1310
url: /zh/python-net/aspose.cells/rowcollection/
is_root: false
---
##  RowCollection类
收集代表工作表中各行的 [Row](/cells/zh/python-net/aspose.cells/row) 对象。



RowCollection 类型公开了以下成员：

### 特性
|属性|描述|
| :- | :- |
| [count](/cells/zh/python-net/aspose.cells/rowcollection/count) |获取此集合中的行数。|



通过给定的行索引获取 [Row](/cells/zh/python-net/aspose.cells/row) 对象。如果给定行索引的 Row 对象之前不存在，则将其实例化。
### 索引器
|名称|描述|
| :- | :- |
| [index] |  |


### 方法
|方法|描述|
| :- | :- |
| [get_row_by_index(index)](/cells/zh/python-net/aspose.cells/rowcollection/get_row_by_index/#int) |根据列表中的位置获取行对象。|
| [clear()](/cells/zh/python-net/aspose.cells/rowcollection/clear/#) |清除所有行和单元格。|
| [remove_at(index)](/cells/zh/python-net/aspose.cells/rowcollection/remove_at/#int) |删除指定索引处的行|



### 例子

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Get first row
row = worksheet.cells.rows[0]

```

### 也可以看看
* 模块 [aspose.cells](..)
* 类 [Row](/cells/zh/python-net/aspose.cells/row)
