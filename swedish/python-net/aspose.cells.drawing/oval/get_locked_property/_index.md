---
title: get_locked_property metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 110
url: /sv/python-net/aspose.cells.drawing/oval/get_locked_property/
is_root: false
---
##  get_locked_property(type) {#ShapeLockType}
Får värdet av låst egendom.


###  Returnerar

Returnerar värdet på låst egendom.


```python
def get_locked_property(self, type):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| type | [ShapeLockType](/cells/sv/python-net/aspose.cells.drawing/shapelocktype) | Typen av formlåst egenskap.|

###  Exempel

```python
from aspose.cells.drawing import ShapeLockType

noAdjustHandles = 0
if shape.get_locked_property(ShapeLockType.ADJUST_HANDLES):
    noAdjustHandles = 1

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [Oval](/cells/sv/python-net/aspose.cells.drawing/oval)
