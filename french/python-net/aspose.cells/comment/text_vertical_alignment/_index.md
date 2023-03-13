---
title: text_vertical_alignment propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 210
url: /fr/python-net/aspose.cells/comment/text_vertical_alignment/
is_root: false
---
##  text_vertical_alignment propriété

Obtient et définit le type d'alignement vertical du texte du commentaire.

###  Exemple

```python
from aspose.cells import TextAlignmentType

if comment1.text_vertical_alignment == TextAlignmentType.FILL:
    comment1.text_vertical_alignment = TextAlignmentType.CENTER

```
###  Définition:
```python
@property
def text_vertical_alignment(self):
    ...
@text_vertical_alignment.setter
def text_vertical_alignment(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [Comment](/cells/fr/python-net/aspose.cells/comment)
* classe [TextAlignmentType](/cells/fr/python-net/aspose.cells/textalignmenttype)
