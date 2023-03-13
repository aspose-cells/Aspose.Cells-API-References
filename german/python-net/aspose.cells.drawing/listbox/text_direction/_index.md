---
title: text_direction Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1010
url: /de/python-net/aspose.cells.drawing/listbox/text_direction/
is_root: false
---
##  text_direction Eigentum

Ruft die Richtung des Textflusses für dieses Objekt ab/legt sie fest.

###  Beispiel

```python
from aspose.cells import TextDirectionType

if shape.text_direction == TextDirectionType.CONTEXT:
    shape.text_direction = TextDirectionType.LEFT_TO_RIGHT

```
###  Definition:
```python
@property
def text_direction(self):
    ...
@text_direction.setter
def text_direction(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ListBox](/cells/de/python-net/aspose.cells.drawing/listbox)
* Klasse [TextDirectionType](/cells/de/python-net/aspose.cells/textdirectiontype)
