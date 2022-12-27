---
title: filter method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 90
url: /python-net/aspose.cells/autofilter/filter/
is_root: false
---

## filter(field_index, criteria) {#int-str}

Filters a list with specified criteria.



```python
def filter(self, field_index, criteria):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| field_index | int | The integer offset of the field on which you want to base the filter <br/>(from the left of the list; the leftmost field is field 0). |
| criteria | str | The specified criteria (a string; for example, "101"). |
### Remarks

Aspose.Cells will remove all other filter setting on this field as Ms Excel 97-2003.


### See Also
* module [aspose.cells](../../)
* class [AutoFilter](/cells/python-net/aspose.cells/autofilter)
