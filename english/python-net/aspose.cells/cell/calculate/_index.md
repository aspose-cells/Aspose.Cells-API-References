---
title: calculate method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 20
url: /python-net/aspose.cells/cell/calculate/
is_root: false
---

## calculate(options) {#CalculationOptions}

Calculates the formula of the cell.



```python
def calculate(self, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| options | [CalculationOptions](/cells/python-net/aspose.cells/calculationoptions) | Options for calculation |


## calculate(ignore_error, custom_function) {#bool-ICustomFunction}

Calculates the formula of the cell.



```python
def calculate(self, ignore_error, custom_function):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| ignore_error | bool | Indicates if hide the error in calculating formulas.<br/>The error may be unsupported function, external links, etc. |
| custom_function | [ICustomFunction](/cells/python-net/aspose.cells/icustomfunction) | The custom formula calculation functions to extend the calculation engine. |
### Remarks

NOTE: This member is now obsolete. Instead, 
please use Calculate(CalculationOptions) method.
This method will be removed 12 months later since August 2020. 
Aspose apologizes for any inconvenience you may have experienced.


### See Also
* module [aspose.cells](../../)
* class [Cell](/cells/python-net/aspose.cells/cell)
