---
title: set_dynamic_array_formula方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 310
url: /zh/python-net/aspose.cells/cell/set_dynamic_array_formula/
is_root: false
---
##  set_dynamic_array_formula(array_formula, options, calculate_value) {#str-FormulaParseOptions-bool}
设置动态数组公式并尽可能使公式溢出到相邻的单元格中。


### 返回

公式应溢出的范围。


```python
def set_dynamic_array_formula(self, array_formula, options, calculate_value):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| array_formula | str |公式表达式|
| options | [FormulaParseOptions](/cells/zh/python-net/aspose.cells/formulaparseoptions) |解析公式的选项。<br/> “解析”选项将被忽略，公式将始终被立即解析|
| calculate_value | bool |是否为溢出范围内的那些单元格计算此动态数组公式。|


##  set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value) {#str-FormulaParseOptions-list-bool-bool}
设置动态数组公式并尽可能使公式溢出到相邻的单元格中。


### 返回

公式应溢出的范围。


```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| array_formula | str |公式表达式|
| options | [FormulaParseOptions](/cells/zh/python-net/aspose.cells/formulaparseoptions) |解析公式的选项。<br/> “解析”选项将被忽略，公式将始终被立即解析|
| values | list |具有给定动态数组公式的那些单元格的值|
| calculate_range | bool |是否计算此动态数组公式的溢出范围。<br/>如果“values”参数不为 null 且此标志为 false，<br/>那么溢出范围的高度将是 values.Length 和 width 将是 values[0].Length。|
| calculate_value | bool |当“values”为空时，是否为溢出范围内的单元格计算此动态数组公式<br/>或一个单元格的“值”中的相应项目为空。|


##  set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value, copts) {#str-FormulaParseOptions-list-bool-bool-CalculationOptions}
设置动态数组公式并尽可能使公式溢出到相邻的单元格中。


### 返回

公式应溢出的范围。


```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value, copts):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| array_formula | str |公式表达式|
| options | [FormulaParseOptions](/cells/zh/python-net/aspose.cells/formulaparseoptions) |解析公式的选项。<br/> “解析”选项将被忽略，公式将始终被立即解析|
| values | list |具有给定动态数组公式的那些单元格的值|
| calculate_range | bool |是否计算此动态数组公式的溢出范围。<br/>如果“values”参数不为 null 且此标志为 false，<br/>那么溢出范围的高度将是 values.Length 和 width 将是 values[0].Length。|
| calculate_value | bool |当“values”为空时，是否为溢出范围内的单元格计算此动态数组公式<br/>或一个单元格的“值”中的相应项目为空。|
| copts | [CalculationOptions](/cells/zh/python-net/aspose.cells/calculationoptions) |计算公式的选项。<br/>通常，出于性能考虑，[CalculationOptions.recursive](/cells/zh/python-net/aspose.cells/calculationoptions#recursive) 属性应为 false。|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Cell](/cells/zh/python-net/aspose.cells/cell)
