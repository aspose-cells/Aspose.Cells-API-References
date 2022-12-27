---
title: get_dependents_in_calculation method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 100
url: /python-net/aspose.cells/cell/get_dependents_in_calculation/
is_root: false
---

## get_dependents_in_calculation(recursive) {#bool}

Gets all cells whose calculated result depends on this cell.

### Returns 


Enumerator to enumerate all dependents(Cell objects)


```python
def get_dependents_in_calculation(self, recursive):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| recursive | bool | Whether returns those dependents which do not reference to this cell directly<br/>but reference to other leafs of this cell |
### Remarks

To use this method, please make sure the workbook has been set with true value for
[FormulaSettings.enable_calculation_chain](/cells/python-net/aspose.cells/formulasettings#enable_calculation_chain) and has been fully calculated with this setting.
If there is no formula reference to this cell, null will be returned.


### See Also
* module [aspose.cells](../../)
* class [Cell](/cells/python-net/aspose.cells/cell)
