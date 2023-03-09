---
title: active_x_control mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 240
url: /tr/python-net/aspose.cells.drawing/rectangleshape/active_x_control/
is_root: false
---
##  active_x_control mülk

ActiveX denetimini alır.

###  örnekler

```python
from aspose import pycore
from aspose.cells.drawing.activexcontrols import CheckBoxActiveXControl

checkBox1 = pycore.cast(CheckBoxActiveXControl, shape.active_x_control)
# The font name of CheckBox
fontName = checkBox1.font.name

```
###  Tanım:
```python
@property
def active_x_control(self):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [ActiveXControl](/cells/tr/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* sınıf [RectangleShape](/cells/tr/python-net/aspose.cells.drawing/rectangleshape)
