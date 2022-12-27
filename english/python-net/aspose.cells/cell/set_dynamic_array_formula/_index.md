---
title: set_dynamic_array_formula method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 310
url: /python-net/aspose.cells/cell/set_dynamic_array_formula/
is_root: false
---

## set_dynamic_array_formula(array_formula, options, calculate_value) {#str-FormulaParseOptions-bool}

Sets dynamic array formula and make the formula spill into neighboring cells if possible.

### Returns 


the range that the formula should spill into.


```python
def set_dynamic_array_formula(self, array_formula, options, calculate_value):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| array_formula | str | the formula expression |
| options | [FormulaParseOptions](/cells/python-net/aspose.cells/formulaparseoptions) | options to parse formula.<br/>"Parse" option will be ignored and the formula will always be parsed immediately |
| calculate_value | bool | whether calculate this dynamic array formula for those cells in the spilled range. |


## set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value) {#str-FormulaParseOptions-list-bool-bool}



```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| array_formula | str |  |
| options | [FormulaParseOptions](/cells/python-net/aspose.cells/formulaparseoptions) |  |
| values | list |  |
| calculate_range | bool |  |
| calculate_value | bool |  |


## set_dynamic_array_formula(array_formula, options, values, calculate_range, calculate_value, copts) {#str-FormulaParseOptions-list-bool-bool-CalculationOptions}



```python
def set_dynamic_array_formula(self, array_formula, options, values, calculate_range, calculate_value, copts):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| array_formula | str |  |
| options | [FormulaParseOptions](/cells/python-net/aspose.cells/formulaparseoptions) |  |
| values | list |  |
| calculate_range | bool |  |
| calculate_value | bool |  |
| copts | [CalculationOptions](/cells/python-net/aspose.cells/calculationoptions) |  |



### See Also
* module [aspose.cells](../../)
* class [Cell](/cells/python-net/aspose.cells/cell)
