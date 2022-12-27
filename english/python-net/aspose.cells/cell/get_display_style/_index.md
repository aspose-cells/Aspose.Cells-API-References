---
title: get_display_style method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 110
url: /python-net/aspose.cells/cell/get_display_style/
is_root: false
---

## get_display_style() {#}

Gets the display style of the cell.
If this cell is also affected by other settings such as conditional formatting, list objects, etc.,
then the display style may be different from cell.GetStyle().



```python
def get_display_style(self):
    ...
```




## get_display_style(include_merged_borders) {#bool}

Gets the display style of the cell.
If the cell is conditional formatted, the display style is not same as the cell.GetStyle().



```python
def get_display_style(self, include_merged_borders):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| include_merged_borders | bool | Indicates whether checking borders of the merged cells. |



### See Also
* module [aspose.cells](../../)
* class [Cell](/cells/python-net/aspose.cells/cell)
