---
title: refresh_dynamic_array_formulas method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 270
url: /python-net/aspose.cells/workbook/refresh_dynamic_array_formulas/
is_root: false
---

## refresh_dynamic_array_formulas(calculate) {#bool}

Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data)
Other formulas in the workbook will not be calculated recursively even if they were used by dynamic array formulas.



```python
def refresh_dynamic_array_formulas(self, calculate):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| calculate | bool | Whether calculates and updates cell values for those dynamic array formulas |


## refresh_dynamic_array_formulas(calculate, copts) {#bool-CalculationOptions}

Refreshes dynamic array formulas(spill into new range of neighboring cells according to current data)



```python
def refresh_dynamic_array_formulas(self, calculate, copts):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| calculate | bool | Whether calculates and updates cell values for those dynamic array formulas |
| copts | [CalculationOptions](/cells/python-net/aspose.cells/calculationoptions) | The options for calculating formulas |



### See Also
* module [aspose.cells](../../)
* class [Workbook](/cells/python-net/aspose.cells/workbook)
