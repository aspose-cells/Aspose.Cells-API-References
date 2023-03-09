---
title: text_horizontal_alignment propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 190
url: /fr/python-net/aspose.cells/comment/text_horizontal_alignment/
is_root: false
---
##  text_horizontal_alignment propriété

Obtient et définit le type d'alignement horizontal du texte du commentaire.

###  Exemple

```python
from aspose.cells import TextAlignmentType

if comment1.text_horizontal_alignment == TextAlignmentType.FILL:
    comment1.text_horizontal_alignment = TextAlignmentType.CENTER

```
###  Définition:
```python
@property
def text_horizontal_alignment(self):
    ...
@text_horizontal_alignment.setter
def text_horizontal_alignment(self, value):
    ...
```

###  Voir également
* module [aspose.cells](../../)
* classe [Comment](/cells/fr/python-net/aspose.cells/comment)
* classe [TextAlignmentType](/cells/fr/python-net/aspose.cells/textalignmenttype)
