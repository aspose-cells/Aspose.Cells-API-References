---
title: text_direction propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 940
url: /es/python-net/aspose.cells.drawing/commentshape/text_direction/
is_root: false
---
##  text_direction propiedad

Obtiene/Establece la dirección del flujo de texto para este objeto.

###  Ejemplo

```python
from aspose.cells import TextDirectionType

if shape.text_direction == TextDirectionType.CONTEXT:
    shape.text_direction = TextDirectionType.LEFT_TO_RIGHT

```
###  Definición:
```python
@property
def text_direction(self):
    ...
@text_direction.setter
def text_direction(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [CommentShape](/cells/es/python-net/aspose.cells.drawing/commentshape)
* clase [TextDirectionType](/cells/es/python-net/aspose.cells/textdirectiontype)
