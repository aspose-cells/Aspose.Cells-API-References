---
title: add_condition method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 40
url: /python-net/aspose.cells/formatconditioncollection/add_condition/
is_root: false
---

## add_condition(type) {#FormatConditionType}

Add a format condition.


### Returns 


Formatting condition object index;


```python
def add_condition(self, type):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| type | [FormatConditionType](/cells/python-net/aspose.cells/formatconditiontype) | Format condition type. |


## add_condition(type, operator_type, formula1, formula2) {#FormatConditionType-OperatorType-str-str}

Adds a formatting condition.


### Returns 


Formatting condition object index;


```python
def add_condition(self, type, operator_type, formula1, formula2):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| type | [FormatConditionType](/cells/python-net/aspose.cells/formatconditiontype) | [FormatConditionType](/cells/python-net/aspose.cells/formatconditiontype) of conditional formatting.<br/>It could be one of the members of FormatConditionType. |
| operator_type | [OperatorType](/cells/python-net/aspose.cells/operatortype) | The comparison [OperatorType](/cells/python-net/aspose.cells/operatortype).<br/>It could be one of the members of OperatorType. |
| formula1 | str | The value or expression associated with conditional formatting.<br/>If the input value starts with '=', then it will be taken as formula.<br/>Otherwise it will be taken as plain value(text, number, bool).<br/>For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| formula2 | str | The value or expression associated with conditional formatting.<br/>The input format is same with formula1 |



### See Also
* module [aspose.cells](../../)
* class [FormatConditionCollection](/cells/python-net/aspose.cells/formatconditioncollection)
* class [FormatConditionType](/cells/python-net/aspose.cells/formatconditiontype)
* class [OperatorType](/cells/python-net/aspose.cells/operatortype)
