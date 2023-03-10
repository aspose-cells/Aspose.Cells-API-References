---
title: check_font_compatibility propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 50
url: /es/python-net/aspose.cells/xpssaveoptions/check_font_compatibility/
is_root: false
---
##  check_font_compatibility propiedad

Indica si se debe comprobar la compatibilidad de fuentes para cada carácter del texto.

###  Observaciones

El valor por defecto es verdadero.
Deshabilitar esta propiedad puede dar un mejor rendimiento.
Pero cuando la fuente predeterminada o especificada de texto/carácter no se puede usar para representarlo,
Es posible que aparezcan caracteres ilegibles (como un bloque) en el pdf generado.
Para tal situación, el usuario debe mantener esta propiedad como verdadera para que
se puede buscar una fuente alternativa y usarla para representar el texto en su lugar;
###  Definición:
```python
@property
def check_font_compatibility(self):
    ...
@check_font_compatibility.setter
def check_font_compatibility(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [XpsSaveOptions](/cells/es/python-net/aspose.cells/xpssaveoptions)
