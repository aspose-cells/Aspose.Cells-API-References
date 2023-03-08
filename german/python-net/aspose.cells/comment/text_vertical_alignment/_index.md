---
title: text_vertical_alignment Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 210
url: /de/python-net/aspose.cells/comment/text_vertical_alignment/
is_root: false
---
##  text_vertical_alignment Eigentum

Ruft den vertikalen Textausrichtungstyp des Kommentars ab und legt diesen fest.

###  Beispiel

```python
from aspose.cells import TextAlignmentType

if comment1.text_vertical_alignment == TextAlignmentType.FILL:
    comment1.text_vertical_alignment = TextAlignmentType.CENTER

```
###  Definition:
```python
@property
def text_vertical_alignment(self):
    ...
@text_vertical_alignment.setter
def text_vertical_alignment(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells](../../)
* Klasse [Comment](/cells/de/python-net/aspose.cells/comment)
* Klasse [TextAlignmentType](/cells/de/python-net/aspose.cells/textalignmenttype)
