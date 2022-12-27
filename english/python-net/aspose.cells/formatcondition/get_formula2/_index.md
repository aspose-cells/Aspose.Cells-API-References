---
title: get_formula2 method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 30
url: /python-net/aspose.cells/formatcondition/get_formula2/
is_root: false
---

## get_formula2(is_r1c1, is_local) {#bool-bool}

Gets the value or expression associated with this format condition.

### Returns 


The value or expression associated with this format condition.


```python
def get_formula2(self, is_r1c1, is_local):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| is_r1c1 | bool | Whether the formula needs to be formatted as R1C1. |
| is_local | bool | Whether the formula needs to be formatted by locale. |


## get_formula2(row, column) {#int-int}

Gets the formula of the conditional formatting of the cell.

### Returns 


The formula.


```python
def get_formula2(self, row, column):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| row | int | The row index. |
| column | int | The column index. |


## get_formula2(is_r1c1, is_local, row, column) {#bool-bool-int-int}

Gets the value or expression of the conditional formatting of the cell.

### Returns 


The value or expression associated with the conditional formatting of the cell.


```python
def get_formula2(self, is_r1c1, is_local, row, column):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| is_r1c1 | bool | Whether the formula needs to be formatted as R1C1. |
| is_local | bool | Whether the formula needs to be formatted by locale. |
| row | int | The row index. |
| column | int | The column index. |
### Remarks

The given cell must be contained by this conditional formatting, otherwise null will be returned.


### See Also
* module [aspose.cells](../../)
* class [FormatCondition](/cells/python-net/aspose.cells/formatcondition)
