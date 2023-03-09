---
title: add_area方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells/validation/add_area/
is_root: false
---
##  add_area(cell_area) {#CellArea}
将验证应用于该区域。



```python
def add_area(self, cell_area):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| cell_area | [CellArea](/cells/zh/python-net/aspose.cells/cellarea) |该地区。|
### 评论

相当于使用[Validation.add_area(cell_area)](/cells/zh/python-net/aspose.cells/validation/add_area)
检查交叉点和边缘。

##  add_area(cell_area, check_intersection, check_edge) {#CellArea-bool-bool}
将验证应用于该区域。



```python
def add_area(self, cell_area, check_intersection, check_edge):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| cell_area | [CellArea](/cells/zh/python-net/aspose.cells/cellarea) |该地区。|
| check_intersection | bool |是否检查给定区域与现有验证区域的交集。<br/>如果在给定区域（或部分区域）应用了一项验证，<br/>那么现有的验证应该首先从给定区域中删除。<br/>否则，生成的验证可能会导致损坏。<br/>如果用户确定添加的区域不与任何现有区域相交，<br/>出于性能考虑，可以将此参数设置为 false。|
| check_edge | bool |是否勾选本次验证应用区域的边缘。<br/>验证的内部设置取决于其应用范围的左上角之一，<br/>因此，如果给定区域将成为新的左上角应用范围之一，<br/>应更改并重建内部设置，否则可能会导致意外结果。<br/>如果用户确定添加的区域不是左上角的区域，<br/>出于性能考虑，可以将此参数设置为 false。|
### 评论

在此方法中，我们将删除给定区域中的所有旧验证。
对于左上角的Validation应用范围，首先它的StartRow最小，
其次，它的 StartColumn 是那些具有相同最小 StartRow 的区域中最小的一个。


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Validation](/cells/zh/python-net/aspose.cells/validation)
