---
title: remove_filter method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 160
url: /python-net/aspose.cells/autofilter/remove_filter/
is_root: false
---

## remove_filter(field_index) {#int}

Remove the specific filter.



```python
def remove_filter(self, field_index):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| field_index | int | The specific filter index |


## remove_filter(field_index, criteria) {#int-str}

Removes a filter for a filter column.



```python
def remove_filter(self, field_index, criteria):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| field_index | int | The integer offset of the field on which you want to base the filter <br/>(from the left of the list; the leftmost field is field 0). |
| criteria | str | The specified criteria (a string; for example, "101"). <br/>It only can be null or be one of the cells' value in this column. |



### See Also
* module [aspose.cells](../../)
* class [AutoFilter](/cells/python-net/aspose.cells/autofilter)
