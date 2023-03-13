---
title: get_leafs方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 160
url: /zh/python-net/aspose.cells/cell/get_leafs/
is_root: false
---
##  get_leafs() {#}
获取直接引用此单元格且需要在修改此单元格时更新的所有单元格。


### 返回

枚举所有家属的枚举器（Cell）


```python
def get_leafs(self):
    ...
```


### 评论

注意：此类现在已过时。反而，
请使用 Cell.GetDependentsInCalculation(bool) 获取计算链中的所有依赖项。
自 2022 年 5 月起，此属性将在 12 个月后移除。
Aspose 对您可能遇到的任何不便深表歉意。

##  get_leafs(recursive) {#bool}
获取修改此单元格时将更新的所有单元格。


### 返回

枚举所有家属的枚举器（Cell）


```python
def get_leafs(self, recursive):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| recursive | bool |是否返回那些不直接引用该单元格的叶子<br/>但引用此单元格的其他叶子|
### 评论

注意：此类现在已过时。反而，
请使用 Cell.GetDependentsInCalculation(bool) 获取计算链中的所有依赖项。
自 2022 年 5 月起，此属性将在 12 个月后移除。
Aspose 对您可能遇到的任何不便深表歉意。


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Cell](/cells/zh/python-net/aspose.cells/cell)
