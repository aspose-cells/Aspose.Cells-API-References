---
title: text_vertical_overflow Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 1020
url: /de/python-net/aspose.cells.drawing/shape/text_vertical_overflow/
is_root: false
---
##  text_vertical_overflow Eigentum

Ruft den vertikalen Textüberlauftyp der Form ab, die Text enthält, und legt diesen fest.

###  Beispiel

```python
from aspose.cells.drawing import TextOverflowType

if shape.text_vertical_overflow == TextOverflowType.CLIP:
    shape.text_vertical_overflow = TextOverflowType.OVERFLOW

```
###  Definition:
```python
@property
def text_vertical_overflow(self):
    ...
@text_vertical_overflow.setter
def text_vertical_overflow(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [Shape](/cells/de/python-net/aspose.cells.drawing/shape)
* Klasse [TextOverflowType](/cells/de/python-net/aspose.cells.drawing/textoverflowtype)
