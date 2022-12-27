---
title: calculate_data method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 40
url: /python-net/aspose.cells.pivot/pivottable/calculate_data/
is_root: false
---

## calculate_data() {#}

Calculates pivottable's data to cells.



```python
def calculate_data(self):
    ...
```


### Remarks

Cell.Value in the pivot range could not return the correct result if the method is not been called.
This method calculates data with an inner pivot cache,not original data source.
So if the data source is changed, please call RefreshData() method first.


### See Also
* module [aspose.cells.pivot](../../)
* class [PivotTable](/cells/python-net/aspose.cells.pivot/pivottable)
