---
title: set_formulas method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 60
url: /python-net/aspose.cells/formatcondition/set_formulas/
is_root: false
---

## set_formulas(formula1, formula2, is_r1c1, is_local) {#str-str-bool-bool}

Sets the value or expression associated with this format condition.



```python
def set_formulas(self, formula1, formula2, is_r1c1, is_local):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| formula1 | str | The value or expression associated with this format condition.<br/>If the input value starts with '=', then it will be taken as formula. Otherwise it will be taken as plain value(text, number, bool).<br/>For text value that starts with '=', user may input it as formula in format: "=\"=...\"". |
| formula2 | str | The value or expression associated with this format condition. The input format is same with formula1 |
| is_r1c1 | bool | Whether the formula is R1C1 formula. |
| is_local | bool | Whether the formula is locale formatted. |



### See Also
* module [aspose.cells](../../)
* class [FormatCondition](/cells/python-net/aspose.cells/formatcondition)
