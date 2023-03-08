---
title: text_horizontal_alignment Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 190
url: /de/python-net/aspose.cells/comment/text_horizontal_alignment/
is_root: false
---
##  text_horizontal_alignment Eigentum

Ruft den horizontalen Textausrichtungstyp des Kommentars ab und legt diesen fest.

###  Beispiel

```python
from aspose.cells import TextAlignmentType

if comment1.text_horizontal_alignment == TextAlignmentType.FILL:
    comment1.text_horizontal_alignment = TextAlignmentType.CENTER

```
###  Definition:
```python
@property
def text_horizontal_alignment(self):
    ...
@text_horizontal_alignment.setter
def text_horizontal_alignment(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Comment](/cells/de/python-net/aspose.cells/comment)
* Klasse [TextAlignmentType](/cells/de/python-net/aspose.cells/textalignmenttype)
