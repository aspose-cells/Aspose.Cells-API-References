---
title: find_formula_contains method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 310
url: /python-net/aspose.cells/cells/find_formula_contains/
is_root: false
---

## find_formula_contains(formula, previous_cell) {#str-Cell}

Finds the cell with formula which contains the input string.

### Returns 


Cell object.


```python
def find_formula_contains(self, formula, previous_cell):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| formula | str | The formula to search for. |
| previous_cell | [Cell](/cells/python-net/aspose.cells/cell) | Previous cell with the same formula. This parameter can be set to null if searching from the start. |
### Remarks

Returns null (Nothing) if no cell is found.
NOTE: This member is now obsolete. Instead, 
please use Cells.Find(object,Cell,FindOptions) method with LookInType as LookInType.OnlyFormulas
and LookAtType as LookAtType.Contains. 
This member will be removed 12 months later since November 2018. 
Aspose apologizes for any inconvenience you may have experienced.


### See Also
* module [aspose.cells](../../)
* class [Cells](/cells/python-net/aspose.cells/cells)
