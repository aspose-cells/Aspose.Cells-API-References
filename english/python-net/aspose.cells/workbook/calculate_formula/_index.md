---
title: calculate_formula method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 40
url: /python-net/aspose.cells/workbook/calculate_formula/
is_root: false
---

## calculate_formula() {#}

Calculates the result of formulas.



```python
def calculate_formula(self):
    ...
```


### Remarks

For all supported formulas, please see the list at https://docs.aspose.com/display/cellsnet/Supported+Formula+Functions

## calculate_formula(ignore_error) {#bool}

Calculates the result of formulas.



```python
def calculate_formula(self, ignore_error):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| ignore_error | bool | Indicates if hide the error in calculating formulas. The error may be unsupported function, external links, etc. |


## calculate_formula(options) {#CalculationOptions}

Calculating formulas in this workbook.



```python
def calculate_formula(self, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| options | [CalculationOptions](/cells/python-net/aspose.cells/calculationoptions) | Options for calculation |


## calculate_formula(ignore_error, custom_function) {#bool-ICustomFunction}

Calculates the result of formulas.



```python
def calculate_formula(self, ignore_error, custom_function):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| ignore_error | bool | Indicates if hide the error in calculating formulas. The error may be unsupported function, external links, etc. |
| custom_function | [ICustomFunction](/cells/python-net/aspose.cells/icustomfunction) | The custom formula calculation functions to extend the calculation engine. |
### Remarks

NOTE: This member is now obsolete. Instead, 
please use CalculateFormula(CalculationOptions) method.
This method will be removed 12 months later since August 2020. 
Aspose apologizes for any inconvenience you may have experienced.


### See Also
* module [aspose.cells](../../)
* class [Workbook](/cells/python-net/aspose.cells/workbook)
