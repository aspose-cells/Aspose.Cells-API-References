---
title: auto_fit_row方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 60
url: /zh/python-net/aspose.cells/worksheet/auto_fit_row/
is_root: false
---
##  auto_fit_row(row_index) {#int}
自动调整行高。



```python
def auto_fit_row(self, row_index):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| row_index | int |行索引。|
### 评论

AutoFitRow 是一个不精确的函数。

##  auto_fit_row(row_index, first_column, last_column) {#int-int-int}

自动调整行高。



```python
def auto_fit_row(self, row_index, first_column, last_column):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| row_index | int |行索引。|
| first_column | int |第一列索引。|
| last_column | int |最后一列索引。|
### 评论

此方法根据行内一系列单元格中的内容自动调整行。

##  auto_fit_row(row_index, first_column, last_column, options) {#int-int-int-AutoFitterOptions}

自动调整行高。



```python
def auto_fit_row(self, row_index, first_column, last_column, options):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| row_index | int |行索引。|
| first_column | int |第一列索引。|
| last_column | int |最后一列索引。|
| options | [AutoFitterOptions](/cells/zh/python-net/aspose.cells/autofitteroptions) |自动装配选项|
### 评论

此方法根据行内一系列单元格中的内容自动调整行。

##  auto_fit_row(start_row, end_row, start_column, end_column) {#int-int-int-int}

自动调整矩形范围内的行高。



```python
def auto_fit_row(self, start_row, end_row, start_column, end_column):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| start_row | int |开始行索引。|
| end_row | int |结束行索引。|
| start_column | int |开始列索引。|
| end_column | int |结束列索引。|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Worksheet](/cells/zh/python-net/aspose.cells/worksheet)
