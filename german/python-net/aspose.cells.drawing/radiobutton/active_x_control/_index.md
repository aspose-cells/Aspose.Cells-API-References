---
title: active_x_control Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 240
url: /de/python-net/aspose.cells.drawing/radiobutton/active_x_control/
is_root: false
---
##  active_x_control Eigentum

Ruft das ActiveX-Steuerelement ab.

###  Beispiele

```python
from aspose import pycore
from aspose.cells.drawing.activexcontrols import CheckBoxActiveXControl

checkBox1 = pycore.cast(CheckBoxActiveXControl, shape.active_x_control)
# The font name of CheckBox
fontName = checkBox1.font.name

```
###  Definition:
```python
@property
def active_x_control(self):
    ...
```

###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ActiveXControl](/cells/de/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* Klasse [RadioButton](/cells/de/python-net/aspose.cells.drawing/radiobutton)
