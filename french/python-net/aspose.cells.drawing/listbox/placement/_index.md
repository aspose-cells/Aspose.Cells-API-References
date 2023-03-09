---
title: placement propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 860
url: /fr/python-net/aspose.cells.drawing/listbox/placement/
is_root: false
---
##  placement propriété

Représente la manière dont l'objet dessin est attaché aux cellules situées en dessous.
La propriété contrôle le placement d'un objet sur une feuille de calcul.

###  Exemples

```python
from aspose.cells.drawing import PlacementType

if shape.placement == PlacementType.MOVE:
    shape.placement = PlacementType.MOVE_AND_SIZE

```
###  Définition:
```python
@property
def placement(self):
    ...
@placement.setter
def placement(self, value):
    ...
```

###  Voir également
* module [aspose.cells.drawing](../../)
* classe [ListBox](/cells/fr/python-net/aspose.cells.drawing/listbox)
* classe [PlacementType](/cells/fr/python-net/aspose.cells.drawing/placementtype)
