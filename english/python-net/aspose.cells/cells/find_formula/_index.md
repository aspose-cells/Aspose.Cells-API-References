---
title: find_formula method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 300
url: /python-net/aspose.cells/cells/find_formula/
is_root: false
---

## find_formula(formula, previous_cell) {#str-Cell}

Finds the cell with the input string.

### Returns 


Cell object.


```python
def find_formula(self, formula, previous_cell):
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
and LookAtType as LookAtType.EntireContent. 
This member will be removed 12 months later since November 2018. 
Aspose apologizes for any inconvenience you may have experienced.


### See Also
* module [aspose.cells](../../)
* class [Cells](/cells/python-net/aspose.cells/cells)
