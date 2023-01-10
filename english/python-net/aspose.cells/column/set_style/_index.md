---
title: set_style method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 40
url: /python-net/aspose.cells/column/set_style/
is_root: false
---

## set_style(style) {#Style}

Sets the style of this column.



```python
def set_style(self, style):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| style | [Style](/cells/python-net/aspose.cells/style) | the style to be used as the default style for cells in this column. |
### Remarks

This method only sets the given style as the default style for this column,
without changing the style settings for existing cells in this column.
To update style settings of existing cells to the specified style at the same time,
please use [Column.apply_style(style, flag)](/cells/python-net/aspose.cells/column/apply_style)


### See Also
* module [aspose.cells](../../)
* class [Column](/cells/python-net/aspose.cells/column)
