---
title: get_leafs method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 160
url: /python-net/aspose.cells/cell/get_leafs/
is_root: false
---

## get_leafs() {#}

Get all cells which reference to this cell directly and need to be updated when this cell is modified.


### Returns 


Enumerator to enumerate all dependents(Cell)


```python
def get_leafs(self):
    ...
```


### Remarks

NOTE: This class is now obsolete. Instead, 
please use Cell.GetDependentsInCalculation(bool) to get all dependents in calculation chain.
This property will be removed 12 months later since May 2022.
Aspose apologizes for any inconvenience you may have experienced.

## get_leafs(recursive) {#bool}

Get all cells which will be updated when this cell is modified.


### Returns 


Enumerator to enumerate all dependents(Cell)


```python
def get_leafs(self, recursive):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| recursive | bool | Whether returns those leafs that do not reference to this cell directly<br/>but reference to other leafs of this cell |
### Remarks

NOTE: This class is now obsolete. Instead, 
please use Cell.GetDependentsInCalculation(bool) to get all dependents in calculation chain.
This property will be removed 12 months later since May 2022.
Aspose apologizes for any inconvenience you may have experienced.


### See Also
* module [aspose.cells](../../)
* class [Cell](/cells/python-net/aspose.cells/cell)
