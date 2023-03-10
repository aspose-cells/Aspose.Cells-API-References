---
title: active_x_control proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 260
url: /it/python-net/aspose.cells.drawing/listbox/active_x_control/
is_root: false
---
##  active_x_control proprietà

Ottiene il controllo ActiveX.

###  Esempio

```python
from aspose import pycore
from aspose.cells.drawing.activexcontrols import CheckBoxActiveXControl

checkBox1 = pycore.cast(CheckBoxActiveXControl, shape.active_x_control)
# The font name of CheckBox
fontName = checkBox1.font.name

```
###  Definizione:
```python
@property
def active_x_control(self):
    ...
```

###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ActiveXControl](/cells/it/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* classe [ListBox](/cells/it/python-net/aspose.cells.drawing/listbox)
