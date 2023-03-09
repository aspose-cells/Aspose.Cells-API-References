---
title: metodo get_locked_property
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 110
url: /it/python-net/aspose.cells.drawing/smartartshape/get_locked_property/
is_root: false
---
##  get_locked_property(type) {#ShapeLockType}
Ottiene il valore della proprietà bloccata.


###  ritorna

Restituisce il valore della proprietà bloccata.


```python
def get_locked_property(self, type):
    ...
```


| Parametri| Tipo| Descrizione|
| :- | :- | :- |
| type | [ShapeLockType](/cells/it/python-net/aspose.cells.drawing/shapelocktype) | Il tipo della proprietà bloccata della forma.|

###  Esempi

```python
from aspose.cells.drawing import ShapeLockType

noAdjustHandles = 0
if shape.get_locked_property(ShapeLockType.ADJUST_HANDLES):
    noAdjustHandles = 1

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [SmartArtShape](/cells/it/python-net/aspose.cells.drawing/smartartshape)
