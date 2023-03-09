---
title: text_vertical_overflow propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1020
url: /fr/python-net/aspose.cells.drawing/oval/text_vertical_overflow/
is_root: false
---
##  text_vertical_overflow propriété

Obtient et définit le type de débordement vertical du texte de la forme qui contient du texte.

###  Exemples

```python
from aspose.cells.drawing import TextOverflowType

if shape.text_vertical_overflow == TextOverflowType.CLIP:
    shape.text_vertical_overflow = TextOverflowType.OVERFLOW

```
###  Définition:
```python
@property
def text_vertical_overflow(self):
    ...
@text_vertical_overflow.setter
def text_vertical_overflow(self, value):
    ...
```

###  Voir également
* module [aspose.cells.drawing](../../)
* classe [Oval](/cells/fr/python-net/aspose.cells.drawing/oval)
* classe [TextOverflowType](/cells/fr/python-net/aspose.cells.drawing/textoverflowtype)
