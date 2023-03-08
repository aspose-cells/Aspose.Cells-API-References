---
title: create_range方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 190
url: /zh/python-net/aspose.cells/cells/create_range/
is_root: false
---
##  create_range(address) {#str}
从范围地址创建一个 [Range](/cells/zh/python-net/aspose.cells/range) 对象。


### 返回

一个 [Range](/cells/zh/python-net/aspose.cells/range) 对象


```python
def create_range(self, address):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| address | str |范围的地址。|


##  create_range(upper_left_cell, lower_right_cell) {#str-str}
从一系列单元格创建一个 [Range](/cells/zh/python-net/aspose.cells/range) 对象。


### 返回

一个 [Range](/cells/zh/python-net/aspose.cells/range) 对象


```python
def create_range(self, upper_left_cell, lower_right_cell):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| upper_left_cell | str |左上角的单元格名称。|
| lower_right_cell | str |右下单元格名称。|


##  create_range(first_index, number, is_vertical) {#int-int-bool}
从单元格行或单元格列创建一个 [Range](/cells/zh/python-net/aspose.cells/range) 对象。


### 返回

一个 [Range](/cells/zh/python-net/aspose.cells/range) 对象。


```python
def create_range(self, first_index, number, is_vertical):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| first_index | int |第一行索引或第一列索引，从零开始。|
| number | int |总行数或列数，以一为基础。|
| is_vertical | bool | True - 从单元格列创建的范围。 False - 从单元格行创建的范围。|


##  create_range(first_row, first_column, total_rows, total_columns) {#int-int-int-int}
从一系列单元格创建一个 [Range](/cells/zh/python-net/aspose.cells/range) 对象。


### 返回

一个 [Range](/cells/zh/python-net/aspose.cells/range) 对象


```python
def create_range(self, first_row, first_column, total_rows, total_columns):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| first_row | int |此范围的第一行|
| first_column | int |此范围的第一列|
| total_rows | int |行数|
| total_columns | int |列数|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Cells](/cells/zh/python-net/aspose.cells/cells)
* 类 [Range](/cells/zh/python-net/aspose.cells/range)
