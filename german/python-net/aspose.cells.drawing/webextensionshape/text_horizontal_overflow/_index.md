---
title: text_horizontal_overflow Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 970
url: /de/python-net/aspose.cells.drawing/webextensionshape/text_horizontal_overflow/
is_root: false
---
##  text_horizontal_overflow Eigentum

Ruft den horizontalen Textüberlauftyp der Form ab, die Text enthält, und legt diesen fest.

###  Beispiel

```python
from aspose.cells.drawing import TextOverflowType

if shape.text_horizontal_overflow == TextOverflowType.CLIP:
    shape.text_horizontal_overflow = TextOverflowType.OVERFLOW

```
###  Definition:
```python
@property
def text_horizontal_overflow(self):
    ...
@text_horizontal_overflow.setter
def text_horizontal_overflow(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [TextOverflowType](/cells/de/python-net/aspose.cells.drawing/textoverflowtype)
* Klasse [WebExtensionShape](/cells/de/python-net/aspose.cells.drawing/webextensionshape)
