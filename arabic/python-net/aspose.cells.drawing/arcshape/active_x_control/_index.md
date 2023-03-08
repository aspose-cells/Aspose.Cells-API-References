---
title: active_x_control الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 240
url: /ar/python-net/aspose.cells.drawing/arcshape/active_x_control/
is_root: false
---
##  active_x_control الملكية

يحصل على عنصر تحكم ActiveX.

###  مثال

```python
from aspose import pycore
from aspose.cells.drawing.activexcontrols import CheckBoxActiveXControl

checkBox1 = pycore.cast(CheckBoxActiveXControl, shape.active_x_control)
# The font name of CheckBox
fontName = checkBox1.font.name

```
###  تعريف:
```python
@property
def active_x_control(self):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ActiveXControl](/cells/ar/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* فئة [ArcShape](/cells/ar/python-net/aspose.cells.drawing/arcshape)
