---
title: get_values method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 30
url: /python-net/aspose.cells/referredarea/get_values/
is_root: false
---

## get_values() {#}

Gets cell values in this area.

### Returns 


If this area is invalid, "#REF!" will be returned;
If this area is one single cell, then return the cell value object;
Otherwise return one 2D array for all values in this area.


```python
def get_values(self):
    ...
```




## get_values(calculate_formulas) {#bool}

Gets cell values in this area.

### Returns 


If this area is invalid, "#REF!" will be returned;
If this area is one single cell, then return the cell value object;
Otherwise return one 2D array for all values in this area.


```python
def get_values(self, calculate_formulas):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| calculate_formulas | bool | In this range, if there are some formulas that have not been calculated,<br/>this flag denotes whether those formulas should be calculated recursively |



### See Also
* module [aspose.cells](../../)
* class [ReferredArea](/cells/python-net/aspose.cells/referredarea)
