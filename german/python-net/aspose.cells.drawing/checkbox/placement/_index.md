---
title: placement Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 840
url: /de/python-net/aspose.cells.drawing/checkbox/placement/
is_root: false
---
##  placement Eigentum

Stellt die Art und Weise dar, wie das Zeichnungsobjekt an die darunter liegenden Zellen angehängt ist.
Die Eigenschaft steuert die placement eines Objekts auf einem Arbeitsblatt.

###  Beispiele

```python
from aspose.cells.drawing import PlacementType

if shape.placement == PlacementType.MOVE:
    shape.placement = PlacementType.MOVE_AND_SIZE

```
###  Definition:
```python
@property
def placement(self):
    ...
@placement.setter
def placement(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [CheckBox](/cells/de/python-net/aspose.cells.drawing/checkbox)
* Klasse [PlacementType](/cells/de/python-net/aspose.cells.drawing/placementtype)
