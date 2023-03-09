---
title: text_direction propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 990
url: /fr/python-net/aspose.cells.drawing/arcshape/text_direction/
is_root: false
---
##  text_direction propriété

Obtient/Définit la direction du flux de texte pour cet objet.

###  Exemples

```python
from aspose.cells import TextDirectionType

if shape.text_direction == TextDirectionType.CONTEXT:
    shape.text_direction = TextDirectionType.LEFT_TO_RIGHT

```
###  Définition:
```python
@property
def text_direction(self):
    ...
@text_direction.setter
def text_direction(self, value):
    ...
```

###  Voir également
* module [aspose.cells.drawing](../../)
* classe [ArcShape](/cells/fr/python-net/aspose.cells.drawing/arcshape)
* classe [TextDirectionType](/cells/fr/python-net/aspose.cells/textdirectiontype)
