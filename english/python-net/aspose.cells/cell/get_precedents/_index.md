---
title: get_precedents method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 180
url: /python-net/aspose.cells/cell/get_precedents/
is_root: false
---

## get_precedents() {#}

Gets all references appearing in this cell's formula.

### Returns 


Collection of all references appearing in this cell's formula.


```python
def get_precedents(self):
    ...
```


### Remarks

* Returns null if this is not a formula cell.All references appearing in this cell's formula will be returned no matter they are referenced or not while calculating.
For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating,
it is still taken as the formula's precedents.To get those references which influence the calculation only, please use [Cell.get_precedents_in_calculation()](/cells/python-net/aspose.cells/cell/get_precedents_in_calculation).

* Returns null if this is not a formula cell.All references appearing in this cell's formula will be returned no matter they are referenced or not while calculating.
For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating,
it is still taken as the formula's precedents.To get those references which influence the calculation only, please use [Cell.get_precedents_in_calculation()](/cells/python-net/aspose.cells/cell/get_precedents_in_calculation).

* Returns null if this is not a formula cell.All references appearing in this cell's formula will be returned no matter they are referenced or not while calculating.
For example, although cell A2 in formula "=IF(TRUE,A1,A2)" is not used while calculating,
it is still taken as the formula's precedents.To get those references which influence the calculation only, please use [Cell.get_precedents_in_calculation()](/cells/python-net/aspose.cells/cell/get_precedents_in_calculation).


### See Also
* module [aspose.cells](../../)
* class [Cell](/cells/python-net/aspose.cells/cell)
