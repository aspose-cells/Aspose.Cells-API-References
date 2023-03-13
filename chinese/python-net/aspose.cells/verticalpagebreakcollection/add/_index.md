---
title: add方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells/verticalpagebreakcollection/add/
is_root: false
---
##  add(column) {#int}
向集合添加垂直分页符。


### 返回

[VerticalPageBreak](/cells/zh/python-net/aspose.cells/verticalpagebreak) 对象索引。


```python
def add(self, column):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| column | int | Cell 列索引，从零开始。|
### 评论

分页符添加在单元格的左上角。
请同时设置水平分页符和垂直分页符。

##  add(cell_name) {#str}
向集合添加垂直分页符。


### 返回

[VerticalPageBreak](/cells/zh/python-net/aspose.cells/verticalpagebreak) 对象索引。


```python
def add(self, cell_name):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| cell_name | str | Cell 名称。|
### 评论

分页符添加在单元格的左上角。
请同时设置水平分页符和垂直分页符。

##  add(row, column) {#int-int}
向集合添加垂直分页符。


### 返回

[VerticalPageBreak](/cells/zh/python-net/aspose.cells/verticalpagebreak) 对象索引。


```python
def add(self, row, column):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| row | int | Cell 行索引，从零开始。|
| column | int | Cell 列索引，从零开始。|
### 评论

分页符添加在单元格的左上角。
请同时设置水平分页符和垂直分页符。

##  add(start_row, end_row, column) {#int-int-int}
向集合添加垂直分页符。


### 返回

[VerticalPageBreak](/cells/zh/python-net/aspose.cells/verticalpagebreak) 对象索引。


```python
def add(self, start_row, end_row, column):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| start_row | int |起始行索引，从零开始。|
| end_row | int |结束行索引，从零开始。|
| column | int |列索引，从零开始。|
### 评论

此方法用于 add 打印区域内的垂直分页符。


### 也可以看看

* 模块 [aspose.cells](../../)
* 类 [VerticalPageBreak](/cells/zh/python-net/aspose.cells/verticalpagebreak)
* 类 [VerticalPageBreakCollection](/cells/zh/python-net/aspose.cells/verticalpagebreakcollection)
