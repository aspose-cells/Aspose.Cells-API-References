---
title: placement proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 820
url: /it/python-net/aspose.cells.drawing/dialogbox/placement/
is_root: false
---
##  placement proprietà

Rappresenta il modo in cui l'oggetto di disegno è collegato alle celle sottostanti.
La proprietà controlla il placement di un oggetto in un foglio di lavoro.

###  Esempi

```python
from aspose.cells.drawing import PlacementType

if shape.placement == PlacementType.MOVE:
    shape.placement = PlacementType.MOVE_AND_SIZE

```
###  Definizione:
```python
@property
def placement(self):
    ...
@placement.setter
def placement(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [DialogBox](/cells/it/python-net/aspose.cells.drawing/dialogbox)
* classe [PlacementType](/cells/it/python-net/aspose.cells.drawing/placementtype)
