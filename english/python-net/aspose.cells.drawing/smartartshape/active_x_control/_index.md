---
title: active_x_control property
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 240
url: /python-net/aspose.cells.drawing/smartartshape/active_x_control/
is_root: false
---

## active_x_control property


Gets the ActiveX control.

### Example 


```python
from aspose import pycore
from aspose.cells.drawing.activexcontrols import CheckBoxActiveXControl

checkBox1 = pycore.cast(CheckBoxActiveXControl, shape.active_x_control)
# The font name of CheckBox
fontName = checkBox1.font.name

```
### Definition:
```python
@property
def active_x_control(self):
    ...
```

### See Also
* module [aspose.cells.drawing](../../)
* class [ActiveXControl](/cells/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* class [SmartArtShape](/cells/python-net/aspose.cells.drawing/smartartshape)
