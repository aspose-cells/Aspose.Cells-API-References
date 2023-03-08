---
title: find_formula方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 300
url: /zh/python-net/aspose.cells/cells/find_formula/
is_root: false
---
##  find_formula(formula, previous_cell) {#str-Cell}
查找包含输入字符串的单元格。


### 返回

Cell 对象。


```python
def find_formula(self, formula, previous_cell):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| formula | str |要搜索的公式。|
| previous_cell | [Cell](/cells/zh/python-net/aspose.cells/cell) |具有相同公式的上一个单元格。如果从头开始搜索，这个参数可以设置为空。|
### 评论

如果未找到单元格，则返回 null（无）。
注意：该成员现已过时。反而，
请使用 Cells.Find(object,Cell,FindOptions) 方法和 LookInType 作为 LookInType.OnlyFormulas
 LookAtType 为 LookAtType.EntireContent。
该成员将于 2018 年 11 月起 12 个月后被删除。
Aspose 对您可能遇到的任何不便深表歉意。


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Cells](/cells/zh/python-net/aspose.cells/cells)
