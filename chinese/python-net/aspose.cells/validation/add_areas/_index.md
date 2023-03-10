---
title: add_areas方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 30
url: /zh/python-net/aspose.cells/validation/add_areas/
is_root: false
---
##  add_areas(areas, check_intersection, check_edge) {#list-bool-bool}
将验证应用于给定区域。



```python
def add_areas(self, areas, check_intersection, check_edge):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| areas | list |领域。|
| check_intersection | bool |是否检查给定区域与现有验证区域的交集。<br/>如果在给定区域（或部分区域）应用了一项验证，<br/>那么现有的验证应该首先从给定区域中删除。<br/>否则可能会导致生成的验证损坏。<br/>如果用户确定所有添加的区域都不与任何现有区域相交，<br/>出于性能考虑，可以将此参数设置为 false。|
| check_edge | bool |是否勾选本次验证应用区域的边缘。<br/>验证的内部设置取决于其应用范围的左上角之一，<br/>因此，如果给定区域之一将成为新的左上角应用范围之一，<br/>应更改内部设置并重建，否则可能会导致意外结果。<br/>如果用户确定这些添加的区域都不是左上角，<br/>出于性能考虑，可以将此参数设置为 false。|
### 评论

在此方法中，我们将删除给定区域中的所有旧验证。
对于左上角的Validation应用范围，首先它的StartRow最小，
其次，它的 StartColumn 是那些具有相同最小 StartRow 的区域中最小的一个。


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Validation](/cells/zh/python-net/aspose.cells/validation)
