---
title: set_shared_formula方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 330
url: /zh/python-net/aspose.cells/cell/set_shared_formula/
is_root: false
---
##  set_shared_formula(shared_formula, row_number, column_number) {#str-int-int}
将共享公式设置为一系列单元格。



```python
def set_shared_formula(self, shared_formula, row_number, column_number):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| shared_formula | str |共享公式。|
| row_number | int |填充公式的行数。|
| column_number | int |填充公式的列数。|
### 评论



##  set_shared_formula(shared_formula, row_number, column_number, options) {#str-int-int-FormulaParseOptions}

将共享公式设置为一系列单元格。



```python
def set_shared_formula(self, shared_formula, row_number, column_number, options):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| shared_formula | str |共享公式。|
| row_number | int |填充公式的行数。|
| column_number | int |填充公式的列数。|
| options | [FormulaParseOptions](/cells/zh/python-net/aspose.cells/formulaparseoptions) |解析公式的选项。|


##  set_shared_formula(shared_formula, row_number, column_number, is_r1c1, is_local) {#str-int-int-bool-bool}
将公式设置为一系列单元格。



```python
def set_shared_formula(self, shared_formula, row_number, column_number, is_r1c1, is_local):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| shared_formula | str |共享公式。|
| row_number | int |填充公式的行数。|
| column_number | int |填充公式的列数。|
| is_r1c1 | bool |公式是否为R1C1公式|
| is_local | bool |公式是否为语言环境格式|
### 评论

注意：此类现在已过时。反而，
请使用 Cell.SetSharedFormula(string,int,int,FormulaParseOptions)。
自 2019 年 12 月起 12 个月后，此属性将被删除。
Aspose 对您可能遇到的任何不便深表歉意。

##  set_shared_formula(shared_formula, row_number, column_number, options, values) {#str-int-int-FormulaParseOptions-list}
将共享公式设置为一系列单元格。



```python
def set_shared_formula(self, shared_formula, row_number, column_number, options, values):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| shared_formula | str |共享公式。|
| row_number | int |填充公式的行数。|
| column_number | int |填充公式的列数。|
| options | [FormulaParseOptions](/cells/zh/python-net/aspose.cells/formulaparseoptions) |解析公式的选项。|
| values | list |具有给定共享公式的那些单元格的值|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Cell](/cells/zh/python-net/aspose.cells/cell)
