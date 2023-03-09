---
title: set_array_formula方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 290
url: /zh/python-net/aspose.cells/cell/set_array_formula/
is_root: false
---
##  set_array_formula(array_formula, row_number, column_number) {#str-int-int}
将数组公式（在 ms excel 中通过 CTRL+SHIFT+ENTER 输入的旧数组公式）设置为单元格区域。



```python
def set_array_formula(self, array_formula, row_number, column_number):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| array_formula | str |数组公式。|
| row_number | int |填充数组公式结果的行数。|
| column_number | int |填充数组公式结果的列数。|


##  set_array_formula(array_formula, row_number, column_number, options) {#str-int-int-FormulaParseOptions}
将数组公式设置为单元格区域。



```python
def set_array_formula(self, array_formula, row_number, column_number, options):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| array_formula | str |数组公式。|
| row_number | int |填充数组公式结果的行数。|
| column_number | int |填充数组公式结果的列数。|
| options | [FormulaParseOptions](/cells/zh/python-net/aspose.cells/formulaparseoptions) |解析公式的选项。|


##  set_array_formula(array_formula, row_number, column_number, is_r1c1, is_local) {#str-int-int-bool-bool}
将数组公式设置为单元格区域。



```python
def set_array_formula(self, array_formula, row_number, column_number, is_r1c1, is_local):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| array_formula | str |数组公式。|
| row_number | int |填充数组公式结果的行数。|
| column_number | int |填充数组公式结果的列数。|
| is_r1c1 | bool |公式是否为R1C1公式|
| is_local | bool |公式是否为语言环境格式|
### 评论

注意：此类现在已过时。
请使用 Cell.SetArrayFormula(string,int,int,FormulaParseOptions)。
自 2019 年 12 月起 12 个月后，此属性将被删除。
Aspose 对您可能遇到的任何不便深表歉意。

##  set_array_formula(array_formula, row_number, column_number, options, values) {#str-int-int-FormulaParseOptions-list}
将数组公式设置为单元格区域。



```python
def set_array_formula(self, array_formula, row_number, column_number, options, values):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| array_formula | str |数组公式。|
| row_number | int |填充数组公式结果的行数。|
| column_number | int |填充数组公式结果的列数。|
| options | [FormulaParseOptions](/cells/zh/python-net/aspose.cells/formulaparseoptions) |解析公式的选项。|
| values | list |具有给定数组公式的那些单元格的值|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Cell](/cells/zh/python-net/aspose.cells/cell)
