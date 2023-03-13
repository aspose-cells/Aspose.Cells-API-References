---
title: set_formula方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 320
url: /zh/python-net/aspose.cells/cell/set_formula/
is_root: false
---
##  set_formula(formula, value) {#str-any}
设置公式和公式的值。



```python
def set_formula(self, formula, value):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| formula | str |公式。|
| value | any |公式的值。|


##  set_formula(formula, options, value) {#str-FormulaParseOptions-any}
设置公式和公式的值。



```python
def set_formula(self, formula, options, value):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| formula | str |公式。|
| options | [FormulaParseOptions](/cells/zh/python-net/aspose.cells/formulaparseoptions) |解析公式的选项。|
| value | any |公式的值。|


##  set_formula(formula, is_r1c1, is_local, value) {#str-bool-bool-any}
设置公式和公式的值。



```python
def set_formula(self, formula, is_r1c1, is_local, value):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| formula | str |公式。|
| is_r1c1 | bool |公式是否为R1C1公式。|
| is_local | bool |公式是否为区域设置格式。|
| value | any |公式的值。|
### 评论

注意：此类现在已过时。反而，
请使用 Cell.SetFormula(string,FormulaParseOptions,object)。
自 2019 年 12 月起 12 个月后，此属性将被删除。
Aspose 对您可能遇到的任何不便深表歉意。


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Cell](/cells/zh/python-net/aspose.cells/cell)
