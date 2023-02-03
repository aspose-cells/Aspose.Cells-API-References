---
title: add method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 20
url: /python-net/aspose.cells/formatconditioncollection/add/
is_root: false
---

## add(cell_area, type, operator_type, formula1, formula2) {#CellArea-FormatConditionType-OperatorType-str-str}

Adds a formatting condition and effected cell rang to the FormatConditions
The FormatConditions can contain up to three conditional formats.
References to the other sheets are not allowed in the formulas of conditional formatting.


### Returns 


[0]:Formatting condition object index;[1] Effected cell rang index.


```python
def add(self, cell_area, type, operator_type, formula1, formula2):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| cell_area | [CellArea](/cells/python-net/aspose.cells/cellarea) | Conditional formatted cell range. |
| type | [FormatConditionType](/cells/python-net/aspose.cells/formatconditiontype) | Type of conditional formatting.It could be one of the members of FormatConditionType. |
| operator_type | [OperatorType](/cells/python-net/aspose.cells/operatortype) | Comparison operator.It could be one of the members of OperatorType. |
| formula1 | str | The value or expression associated with conditional formatting. |
| formula2 | str | The value or expression associated with conditional formatting |



### See Also
* module [aspose.cells](../../)
* class [FormatConditionCollection](/cells/python-net/aspose.cells/formatconditioncollection)
