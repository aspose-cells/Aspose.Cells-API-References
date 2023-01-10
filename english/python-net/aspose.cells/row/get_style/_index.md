---
title: get_style method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 70
url: /python-net/aspose.cells/row/get_style/
is_root: false
---

## get_style() {#}

Gets the style of this row.



```python
def get_style(self):
    ...
```


### Remarks

Modifying the returned style object directly takes no effect for this row or any cells in this row.
You have to call [Row.apply_style(style, flag)](/cells/python-net/aspose.cells/row/apply_style) or [Row.set_style(style)](/cells/python-net/aspose.cells/row/set_style) method
to apply the change to this row.

Row's style is the style which will be inherited by cells in this row(those cells that have no custom style settings,
such as existing cells that have not been set style explicitly, or those that have not been instantiated)


### See Also
* module [aspose.cells](../../)
* class [Row](/cells/python-net/aspose.cells/row)
