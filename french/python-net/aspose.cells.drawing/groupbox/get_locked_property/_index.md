---
title: get_locked_property méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 110
url: /fr/python-net/aspose.cells.drawing/groupbox/get_locked_property/
is_root: false
---
##  get_locked_property(type) {#ShapeLockType}
Obtient la valeur de la propriété verrouillée.


###  Retour

Renvoie la valeur de la propriété verrouillée.


```python
def get_locked_property(self, type):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| type | [ShapeLockType](/cells/fr/python-net/aspose.cells.drawing/shapelocktype) | Le type de la propriété verrouillée de la forme.|

###  Exemple

```python
from aspose.cells.drawing import ShapeLockType

noAdjustHandles = 0
if shape.get_locked_property(ShapeLockType.ADJUST_HANDLES):
    noAdjustHandles = 1

```



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [GroupBox](/cells/fr/python-net/aspose.cells.drawing/groupbox)
