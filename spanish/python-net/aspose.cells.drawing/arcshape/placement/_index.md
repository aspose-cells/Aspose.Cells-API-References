---
title: placement propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 880
url: /es/python-net/aspose.cells.drawing/arcshape/placement/
is_root: false
---
##  placement propiedad

Representa la forma en que el objeto de dibujo se adjunta a las celdas debajo de él.
La propiedad controla el placement de un objeto en una hoja de cálculo.

###  Ejemplo

```python
from aspose.cells.drawing import PlacementType

if shape.placement == PlacementType.MOVE:
    shape.placement = PlacementType.MOVE_AND_SIZE

```
###  Definición:
```python
@property
def placement(self):
    ...
@placement.setter
def placement(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ArcShape](/cells/es/python-net/aspose.cells.drawing/arcshape)
* clase [PlacementType](/cells/es/python-net/aspose.cells.drawing/placementtype)
