---
title: text_vertical_alignment propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 210
url: /es/python-net/aspose.cells/comment/text_vertical_alignment/
is_root: false
---
##  text_vertical_alignment propiedad

Obtiene y establece el tipo de alineación vertical del texto del comentario.

###  Ejemplos

```python
from aspose.cells import TextAlignmentType

if comment1.text_vertical_alignment == TextAlignmentType.FILL:
    comment1.text_vertical_alignment = TextAlignmentType.CENTER

```
###  Definición:
```python
@property
def text_vertical_alignment(self):
    ...
@text_vertical_alignment.setter
def text_vertical_alignment(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [Comment](/cells/es/python-net/aspose.cells/comment)
* clase [TextAlignmentType](/cells/es/python-net/aspose.cells/textalignmenttype)
