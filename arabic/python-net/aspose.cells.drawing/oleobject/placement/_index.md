---
title: placement الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 980
url: /ar/python-net/aspose.cells.drawing/oleobject/placement/
is_root: false
---
##  placement الملكية

يمثل الطريقة التي يتم بها إرفاق الكائن الرسومي بالخلايا الموجودة أسفله.
تتحكم الخاصية في placement لكائن موجود بورقة عمل.

###  مثال

```python
from aspose.cells.drawing import PlacementType

if shape.placement == PlacementType.MOVE:
    shape.placement = PlacementType.MOVE_AND_SIZE

```
###  تعريف:
```python
@property
def placement(self):
    ...
@placement.setter
def placement(self, value):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [OleObject](/cells/ar/python-net/aspose.cells.drawing/oleobject)
* فئة [PlacementType](/cells/ar/python-net/aspose.cells.drawing/placementtype)
