---
title: sort方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 40
url: /zh/python-net/aspose.cells/datasorter/sort/
is_root: false
---
##  sort() {#}
对范围内的数据进行排序。


### 返回

已排序行/列的原始索引（绝对位置，例如，列 A 为 0，B 为 1，...）。
如果此排序操作不需要移动行/列，则返回 null。


```python
def sort(self):
    ...
```




##  sort(cells, area) {#Cells-CellArea}
对区域的数据进行排序。


### 返回

已排序行/列的原始索引（绝对位置，例如，列 A 为 0，B 为 1，...）。
如果此排序操作不需要移动行/列，则返回 null。


```python
def sort(self, cells, area):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| cells | [Cells](/cells/zh/python-net/aspose.cells/cells) |单元格包含数据区域。|
| area | [CellArea](/cells/zh/python-net/aspose.cells/cellarea) |需要排序的区域|


##  sort(cells, start_row, start_column, end_row, end_column) {#Cells-int-int-int-int}
对区域的数据进行排序。


### 返回

已排序行/列的原始索引（绝对位置，例如，列 A 为 0，B 为 1，...）。
如果此排序操作不需要移动行/列，则返回 null。


```python
def sort(self, cells, start_row, start_column, end_row, end_column):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| cells | [Cells](/cells/zh/python-net/aspose.cells/cells) |单元格包含数据区域。|
| start_row | int |区域的起始行。|
| start_column | int |区域的起始列。|
| end_row | int |该区域的末行。|
| end_column | int |该区域的结束列。|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [DataSorter](/cells/zh/python-net/aspose.cells/datasorter)
