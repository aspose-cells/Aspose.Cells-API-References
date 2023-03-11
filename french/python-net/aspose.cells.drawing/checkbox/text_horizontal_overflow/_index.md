---
title: text_horizontal_overflow propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 1000
url: /fr/python-net/aspose.cells.drawing/checkbox/text_horizontal_overflow/
is_root: false
---
##  text_horizontal_overflow propriété

Obtient et définit le type de débordement horizontal du texte de la forme qui contient du texte.

###  Exemple

```python
from aspose.cells.drawing import TextOverflowType

if shape.text_horizontal_overflow == TextOverflowType.CLIP:
    shape.text_horizontal_overflow = TextOverflowType.OVERFLOW

```
###  Définition:
```python
@property
def text_horizontal_overflow(self):
    ...
@text_horizontal_overflow.setter
def text_horizontal_overflow(self, value):
    ...
```

###  Voir également
* module [aspose.cells.drawing](../../)
* classe [CheckBox](/cells/fr/python-net/aspose.cells.drawing/checkbox)
* classe [TextOverflowType](/cells/fr/python-net/aspose.cells.drawing/textoverflowtype)
