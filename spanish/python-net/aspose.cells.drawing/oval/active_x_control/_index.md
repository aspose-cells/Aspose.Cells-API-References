---
title: active_x_control propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 240
url: /es/python-net/aspose.cells.drawing/oval/active_x_control/
is_root: false
---
##  active_x_control propiedad

Obtiene el control ActiveX.

###  Ejemplos

```python
from aspose import pycore
from aspose.cells.drawing.activexcontrols import CheckBoxActiveXControl

checkBox1 = pycore.cast(CheckBoxActiveXControl, shape.active_x_control)
# The font name of CheckBox
fontName = checkBox1.font.name

```
###  Definición:
```python
@property
def active_x_control(self):
    ...
```

###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ActiveXControl](/cells/es/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* clase [Oval](/cells/es/python-net/aspose.cells.drawing/oval)
