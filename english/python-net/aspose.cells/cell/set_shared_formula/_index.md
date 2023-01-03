---
title: set_shared_formula method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 330
url: /python-net/aspose.cells/cell/set_shared_formula/
is_root: false
---

## set_shared_formula(shared_formula, row_number, column_number) {#str-int-int}

Sets shared formulas to a range of cells.



```python
def set_shared_formula(self, shared_formula, row_number, column_number):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| shared_formula | str | Shared formula. |
| row_number | int | Number of rows to populate the formula. |
| column_number | int | Number of columns to populate the formula. |
### Remarks



## set_shared_formula(shared_formula, row_number, column_number, options) {#str-int-int-FormulaParseOptions}

Sets shared formulas to a range of cells.



```python
def set_shared_formula(self, shared_formula, row_number, column_number, options):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| shared_formula | str | Shared formula. |
| row_number | int | Number of rows to populate the formula. |
| column_number | int | Number of columns to populate the formula. |
| options | [FormulaParseOptions](/cells/python-net/aspose.cells/formulaparseoptions) | Options for parsing the formula. |


## set_shared_formula(shared_formula, row_number, column_number, is_r1c1, is_local) {#str-int-int-bool-bool}

Sets a formula to a range of cells.



```python
def set_shared_formula(self, shared_formula, row_number, column_number, is_r1c1, is_local):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| shared_formula | str | Shared formula. |
| row_number | int | Number of rows to populate the formula. |
| column_number | int | Number of columns to populate the formula. |
| is_r1c1 | bool | whether the formula is R1C1 formula |
| is_local | bool | whether the formula is locale formatted |
### Remarks

NOTE: This class is now obsolete. Instead, 
please use Cell.SetSharedFormula(string,int,int,FormulaParseOptions).
This property will be removed 12 months later since December 2019.
Aspose apologizes for any inconvenience you may have experienced.

## set_shared_formula(shared_formula, row_number, column_number, options, values) {#str-int-int-FormulaParseOptions-list}

Sets shared formulas to a range of cells.



```python
def set_shared_formula(self, shared_formula, row_number, column_number, options, values):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| shared_formula | str | Shared formula. |
| row_number | int | Number of rows to populate the formula. |
| column_number | int | Number of columns to populate the formula. |
| options | [FormulaParseOptions](/cells/python-net/aspose.cells/formulaparseoptions) | Options for parsing the formula. |
| values | list | values for those cells with given shared formula |



### See Also
* module [aspose.cells](../../)
* class [Cell](/cells/python-net/aspose.cells/cell)
