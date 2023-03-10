---
title: add_condition方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 40
url: /zh/python-net/aspose.cells/formatconditioncollection/add_condition/
is_root: false
---
##  add_condition(type) {#FormatConditionType}
添加格式条件。


### 返回

格式化条件对象索引；


```python
def add_condition(self, type):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| type | [FormatConditionType](/cells/zh/python-net/aspose.cells/formatconditiontype) |格式条件类型。|


##  add_condition(type, operator_type, formula1, formula2) {#FormatConditionType-OperatorType-str-str}
添加格式化条件。


### 返回

格式化条件对象索引；


```python
def add_condition(self, type, operator_type, formula1, formula2):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| type | [FormatConditionType](/cells/zh/python-net/aspose.cells/formatconditiontype) | [FormatConditionType](/cells/zh/python-net/aspose.cells/formatconditiontype) 条件格式。<br/>它可以是 FormatConditionType 的成员之一。|
| operator_type | [OperatorType](/cells/zh/python-net/aspose.cells/operatortype) |比较 [OperatorType](/cells/zh/python-net/aspose.cells/operatortype)。<br/>它可以是 OperatorType 的成员之一。|
| formula1 | str |与条件格式关联的值或表达式。<br/>如果输入值以'='开头，则将其作为公式。<br/>否则它将被视为纯值（文本、数字、布尔值）。<br/>对于以'='开头的文本值，用户可以将其作为公式输入，格式为："=\"=...\""。|
| formula2 | str |与条件格式关联的值或表达式。<br/>输入格式同公式1|



### 也可以看看
* 模块 [aspose.cells](../../)
* 类 [FormatConditionCollection](/cells/zh/python-net/aspose.cells/formatconditioncollection)
* 类 [FormatConditionType](/cells/zh/python-net/aspose.cells/formatconditiontype)
* 类 [OperatorType](/cells/zh/python-net/aspose.cells/operatortype)
