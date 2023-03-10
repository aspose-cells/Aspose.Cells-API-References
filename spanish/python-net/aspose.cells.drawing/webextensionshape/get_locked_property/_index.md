---
title: get_locked_property método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 110
url: /es/python-net/aspose.cells.drawing/webextensionshape/get_locked_property/
is_root: false
---
##  get_locked_property(type) {#ShapeLockType}
Obtiene el valor de la propiedad bloqueada.


###  Devoluciones

Devuelve el valor de la propiedad bloqueada.


```python
def get_locked_property(self, type):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| type | [ShapeLockType](/cells/es/python-net/aspose.cells.drawing/shapelocktype) | El tipo de la propiedad bloqueada de forma.|

###  Ejemplo

```python
from aspose.cells.drawing import ShapeLockType

noAdjustHandles = 0
if shape.get_locked_property(ShapeLockType.ADJUST_HANDLES):
    noAdjustHandles = 1

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [WebExtensionShape](/cells/es/python-net/aspose.cells.drawing/webextensionshape)
