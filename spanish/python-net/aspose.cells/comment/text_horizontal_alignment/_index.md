---
title: text_horizontal_alignment propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 190
url: /es/python-net/aspose.cells/comment/text_horizontal_alignment/
is_root: false
---
##  text_horizontal_alignment propiedad

Obtiene y establece el tipo de alineación horizontal del texto del comentario.

###  Ejemplo

```python
from aspose.cells import TextAlignmentType

if comment1.text_horizontal_alignment == TextAlignmentType.FILL:
    comment1.text_horizontal_alignment = TextAlignmentType.CENTER

```
###  Definición:
```python
@property
def text_horizontal_alignment(self):
    ...
@text_horizontal_alignment.setter
def text_horizontal_alignment(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [Comment](/cells/es/python-net/aspose.cells/comment)
* clase [TextAlignmentType](/cells/es/python-net/aspose.cells/textalignmenttype)
