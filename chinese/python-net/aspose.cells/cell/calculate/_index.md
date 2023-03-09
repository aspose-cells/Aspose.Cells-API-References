---
title: calculate方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells/cell/calculate/
is_root: false
---
##  calculate(options) {#CalculationOptions}
计算单元格的公式。



```python
def calculate(self, options):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| options | [CalculationOptions](/cells/zh/python-net/aspose.cells/calculationoptions) |计算选项|


##  calculate(ignore_error, custom_function) {#bool-ICustomFunction}
计算单元格的公式。



```python
def calculate(self, ignore_error, custom_function):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| ignore_error | bool |指示是否隐藏计算公式中的错误。<br/>错误可能是不支持的功能、外部链接等。|
| custom_function | [ICustomFunction](/cells/zh/python-net/aspose.cells/icustomfunction) |自定义公式计算功能，扩展计算引擎。|
### 评论

注意：该成员现已过时。
请使用 Calculate(CalculationOptions) 方法。
自 2020 年 8 月起，此方法将在 12 个月后被删除。
Aspose 对您可能遇到的任何不便深表歉意。


### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [Cell](/cells/zh/python-net/aspose.cells/cell)
