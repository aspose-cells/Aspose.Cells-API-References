---
title: set_array_formula method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 290
url: /python-net/aspose.cells/cell/set_array_formula/
is_root: false
---

## set_array_formula(array_formula, row_number, column_number) {#str-int-int}

Sets an array formula(legacy array formula entered via CTRL+SHIFT+ENTER in ms excel) to a range of cells.



```python
def set_array_formula(self, array_formula, row_number, column_number):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| array_formula | str | Array formula. |
| row_number | int | Number of rows to populate result of the array formula. |
| column_number | int | Number of columns to populate result of the array formula. |


## set_array_formula(array_formula, row_number, column_number, options) {#str-int-int-FormulaParseOptions}

Sets an array formula to a range of cells.



```python
def set_array_formula(self, array_formula, row_number, column_number, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| array_formula | str | Array formula. |
| row_number | int | Number of rows to populate result of the array formula. |
| column_number | int | Number of columns to populate result of the array formula. |
| options | [FormulaParseOptions](/cells/python-net/aspose.cells/formulaparseoptions) | Options for parsing the formula. |


## set_array_formula(array_formula, row_number, column_number, is_r1c1, is_local) {#str-int-int-bool-bool}

Sets an array formula to a range of cells.



```python
def set_array_formula(self, array_formula, row_number, column_number, is_r1c1, is_local):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| array_formula | str | Array formula. |
| row_number | int | Number of rows to populate result of the array formula. |
| column_number | int | Number of columns to populate result of the array formula. |
| is_r1c1 | bool | whether the formula is R1C1 formula |
| is_local | bool | whether the formula is locale formatted |
### Remarks

NOTE: This class is now obsolete. Instead, 
please use Cell.SetArrayFormula(string,int,int,FormulaParseOptions).
This property will be removed 12 months later since December 2019.
Aspose apologizes for any inconvenience you may have experienced.

## set_array_formula(array_formula, row_number, column_number, options, values) {#str-int-int-FormulaParseOptions-list}

Sets an array formula to a range of cells.



```python
def set_array_formula(self, array_formula, row_number, column_number, options, values):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| array_formula | str | Array formula. |
| row_number | int | Number of rows to populate result of the array formula. |
| column_number | int | Number of columns to populate result of the array formula. |
| options | [FormulaParseOptions](/cells/python-net/aspose.cells/formulaparseoptions) | Options for parsing the formula. |
| values | list | values for those cells with given array formula |



### See Also
* module [aspose.cells](../../)
* class [Cell](/cells/python-net/aspose.cells/cell)
