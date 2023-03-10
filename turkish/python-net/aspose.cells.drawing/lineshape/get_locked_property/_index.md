---
title: get_locked_property yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 110
url: /tr/python-net/aspose.cells.drawing/lineshape/get_locked_property/
is_root: false
---
##  get_locked_property(type) {#ShapeLockType}
Lock özelliğinin değerini alır.


###  İadeler

Kilitli özelliğin değerini döndürür.


```python
def get_locked_property(self, type):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| type | [ShapeLockType](/cells/tr/python-net/aspose.cells.drawing/shapelocktype) | Şekil kilitli özelliğinin türü.|

###  Örnek

```python
from aspose.cells.drawing import ShapeLockType

noAdjustHandles = 0
if shape.get_locked_property(ShapeLockType.ADJUST_HANDLES):
    noAdjustHandles = 1

```



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [LineShape](/cells/tr/python-net/aspose.cells.drawing/lineshape)
