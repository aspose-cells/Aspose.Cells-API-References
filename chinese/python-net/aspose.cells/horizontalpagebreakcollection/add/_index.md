---
title: add方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells/horizontalpagebreakcollection/add/
is_root: false
---
##  add(row) {#int}
向集合中添加水平分页符。


### 返回

[HorizontalPageBreak](/cells/zh/python-net/aspose.cells/horizontalpagebreak) 对象索引。


```python
def add(self, row):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| row | int | Cell 行索引，从零开始。|
### 评论

分页符添加在单元格的左上角。
请同时设置水平分页符和垂直分页符。

##  add(cell_name) {#str}
向集合中添加水平分页符。


### 返回

[HorizontalPageBreak](/cells/zh/python-net/aspose.cells/horizontalpagebreak) 对象索引。


```python
def add(self, cell_name):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| cell_name | str | Cell 名称。|
### 评论

分页符添加在单元格的左上角。
请同时设置水平分页符和垂直分页符。

##  add(row, column) {#int-int}
向集合中添加水平分页符。


### 返回

[HorizontalPageBreak](/cells/zh/python-net/aspose.cells/horizontalpagebreak) 对象索引。


```python
def add(self, row, column):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| row | int | Cell 行索引，从零开始。|
| column | int | Cell 列索引，从零开始。|
### 评论

分页符添加在单元格的左上角。
请同时设置水平分页符和垂直分页符。

##  add(row, start_column, end_column) {#int-int-int}
向集合中添加水平分页符。


### 返回

[HorizontalPageBreak](/cells/zh/python-net/aspose.cells/horizontalpagebreak) 对象索引。


```python
def add(self, row, start_column, end_column):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| row | int |行索引，从零开始。|
| start_column | int |起始列索引，从零开始。|
| end_column | int |结束列索引，从零开始。|
### 评论

add 此方法用于打印区域内的水平分页符。


### 也可以看看

* 模块 [aspose.cells](../../)
* 类 [HorizontalPageBreak](/cells/zh/python-net/aspose.cells/horizontalpagebreak)
* 类 [HorizontalPageBreakCollection](/cells/zh/python-net/aspose.cells/horizontalpagebreakcollection)
