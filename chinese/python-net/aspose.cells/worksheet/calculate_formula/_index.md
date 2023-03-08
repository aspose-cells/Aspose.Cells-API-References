---
title: calculate_formula方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 80
url: /zh/python-net/aspose.cells/worksheet/calculate_formula/
is_root: false
---
##  calculate_formula(formula) {#str}
计算一个公式。


### 返回

计算公式结果。


```python
def calculate_formula(self, formula):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| formula | str |要计算的公式。|


##  calculate_formula(formula, opts) {#str-CalculationOptions}
计算一个公式。


### 返回

计算公式结果。


```python
def calculate_formula(self, formula, opts):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| formula | str |要计算的公式。|
| opts | [CalculationOptions](/cells/zh/python-net/aspose.cells/calculationoptions) |计算公式选项|


##  calculate_formula(options, recursive) {#CalculationOptions-bool}
计算此工作表中的所有公式。



```python
def calculate_formula(self, options, recursive):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| options | [CalculationOptions](/cells/zh/python-net/aspose.cells/calculationoptions) |计算选项|
| recursive | bool | True 表示如果工作表的单元格依赖于其他工作表的单元格，<br/>其他工作表中的相关单元格也将被计算。<br/> False 表示工作表中的所有公式均已计算且值正确。|


##  calculate_formula(recursive, ignore_error, custom_function) {#bool-bool-ICustomFunction}
计算此工作表中的所有公式。



```python
def calculate_formula(self, recursive, ignore_error, custom_function):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| recursive | bool | True 表示如果工作表的单元格依赖于其他工作表的单元格，<br/>其他工作表中的相关单元格也将被计算。<br/> False 表示工作表中的所有公式均已计算且值正确。|
| ignore_error | bool |指示是否隐藏计算公式中的错误。<br/>错误可能是不支持的功能、外部链接等。|
| custom_function | [ICustomFunction](/cells/zh/python-net/aspose.cells/icustomfunction) |自定义公式计算功能，扩展计算引擎。|
### 评论

注意：该成员现已过时。反而，
请使用 CalculateFormula(CalculationOptions, bool) 方法。
自 2020 年 8 月起，此方法将在 12 个月后被删除。
Aspose 对您可能遇到的任何不便深表歉意。


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Worksheet](/cells/zh/python-net/aspose.cells/worksheet)
