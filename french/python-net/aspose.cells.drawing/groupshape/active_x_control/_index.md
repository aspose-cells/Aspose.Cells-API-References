---
title: active_x_control propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 260
url: /fr/python-net/aspose.cells.drawing/groupshape/active_x_control/
is_root: false
---
##  active_x_control propriété

Obtient le contrôle ActiveX.

###  Exemple

```python
from aspose import pycore
from aspose.cells.drawing.activexcontrols import CheckBoxActiveXControl

checkBox1 = pycore.cast(CheckBoxActiveXControl, shape.active_x_control)
# The font name of CheckBox
fontName = checkBox1.font.name

```
###  Définition:
```python
@property
def active_x_control(self):
    ...
```

###  Voir également
* module [aspose.cells.drawing](../../)
* classe [ActiveXControl](/cells/fr/python-net/aspose.cells.drawing.activexcontrols/activexcontrol)
* classe [GroupShape](/cells/fr/python-net/aspose.cells.drawing/groupshape)
