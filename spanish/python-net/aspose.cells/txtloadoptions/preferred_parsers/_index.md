---
title: preferred_parsers propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 300
url: /es/python-net/aspose.cells/txtloadoptions/preferred_parsers/
is_root: false
---
##  preferred_parsers propiedad

Obtiene y establece los analizadores de valores preferidos para cargar archivos de texto.

###  Observaciones

parsers[0] es el analizador que se usará para la primera columna en el archivo de plantilla de texto,
parsers[1] es el analizador que se usará para la segunda columna, etc.
El último (parsers[parsers.length-1]) se usará para todas las demás columnas a partir de parsers.length-1.
Si un elemento es nulo, la columna correspondiente será analizada por el analizador predeterminado de Aspose.Cells.
###  Definición:
```python
@property
def preferred_parsers(self):
    ...
@preferred_parsers.setter
def preferred_parsers(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [TxtLoadOptions](/cells/es/python-net/aspose.cells/txtloadoptions)
