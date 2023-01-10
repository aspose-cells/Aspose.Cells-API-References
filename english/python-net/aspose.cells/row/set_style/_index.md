---
title: set_style method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 80
url: /python-net/aspose.cells/row/set_style/
is_root: false
---

## set_style(style) {#Style}

Sets the style of this row.



```python
def set_style(self, style):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| style | [Style](/cells/python-net/aspose.cells/style) | the style to be used as the default style for cells in this row. |
### Remarks

This method only sets the given style as the default style for this row,
without changing the style settings for existing cells in this row.
To update style settings of existing cells to the specified style at the same time,
please use [Row.apply_style(style, flag)](/cells/python-net/aspose.cells/row/apply_style)


### See Also
* module [aspose.cells](../../)
* class [Row](/cells/python-net/aspose.cells/row)
