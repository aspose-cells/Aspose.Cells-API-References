---
title: add_filter method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 40
url: /python-net/aspose.cells/autofilter/add_filter/
is_root: false
---

## add_filter(field_index, criteria) {#int-str}

Adds a filter for a filter column.



```python
def add_filter(self, field_index, criteria):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| field_index | int | The integer offset of the field on which you want to base the filter <br/>(from the left of the list; the leftmost field is field 0). |
| criteria | str | The specified criteria (a string; for example, "101"). <br/>It only can be null or be one of the cells' value in this column. |
### Remarks

MS Excel 2007 supports multiple selection in a filter column.


### See Also
* module [aspose.cells](../../)
* class [AutoFilter](/cells/python-net/aspose.cells/autofilter)
