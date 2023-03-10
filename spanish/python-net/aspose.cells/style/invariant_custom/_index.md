---
title: invariant_custom propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 260
url: /es/python-net/aspose.cells/style/invariant_custom/
is_root: false
---
##  invariant_custom propiedad

Obtiene la cadena de patrón independiente de la referencia cultural para el formato de número.
Si no se ha establecido un formato de número para este objeto, se devolverá un valor nulo.
Si el formato de número está integrado, se devolverá la cadena de patrón correspondiente al número integrado.

###  Observaciones

Para los formatos de números integrados, el contenido del patrón devuelto aún depende de la cultura,
por ejemplo, para algunas configuraciones regionales devuelve "m/d/y" y para otras configuraciones regionales devuelve "d/m/y".
La diferencia con [Style.culture_custom](/cells/es/python-net/aspose.cells/style#culture_custom) es (eso es también lo que significa cultura independiente):
los especificadores de formato y los separadores se mantienen como estándar, como '/' siempre se usará como separador de fecha y hora
y "y" siempre se usará como la parte del "año", sin importar qué otro carácter especial se use para el lugar específico.
###  Definición:
```python
@property
def invariant_custom(self):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [Style](/cells/es/python-net/aspose.cells/style)
