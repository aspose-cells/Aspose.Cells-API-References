---
title: culture_custom propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 170
url: /es/python-net/aspose.cells/style/culture_custom/
is_root: false
---
##  culture_custom propiedad

Obtiene y establece la cadena de patrón dependiente de la referencia cultural para el formato de número.
Si no se ha establecido un formato de número para este objeto, se devolverá un valor nulo.
Si el formato de número está integrado, se devolverá la cadena de patrón correspondiente al número integrado.

###  Observaciones

Para el formato de número incorporado, tanto el contenido del patrón (por ejemplo, un formato de fecha incorporado es "m/d/y" para algunas configuraciones regionales,
pero para algunas otras configuraciones regionales se convierte en "d/m/y") y el especificador de formato (como,
algunas configuraciones regionales utilizan un carácter distinto de 'y' para representar la parte del año para el formato de fecha)
dependen de la cultura;
Para el formato personalizado especificado por el usuario, solo los especificadores de formato se cambian de acuerdo con la cultura,
otras partes del patrón de formato no se modificarán.
###  Definición:
```python
@property
def culture_custom(self):
    ...
@culture_custom.setter
def culture_custom(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells](../../)
* clase [Style](/cells/es/python-net/aspose.cells/style)
