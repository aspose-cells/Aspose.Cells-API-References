---
title: طريقة get_locked_property
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 120
url: /ar/python-net/aspose.cells.drawing/picture/get_locked_property/
is_root: false
---
##  get_locked_property(type) {#ShapeLockType}
يحصل على قيمة الممتلكات المقفلة.


###  عائدات

ترجع قيمة الممتلكات المقفلة.


```python
def get_locked_property(self, type):
    ...
```


| حدود| يكتب| وصف|
| :- | :- | :- |
| type | [ShapeLockType](/cells/ar/python-net/aspose.cells.drawing/shapelocktype) | نوع خاصية تأمين الشكل.|

###  أمثلة

```python
from aspose.cells.drawing import ShapeLockType

noAdjustHandles = 0
if shape.get_locked_property(ShapeLockType.ADJUST_HANDLES):
    noAdjustHandles = 1

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [Picture](/cells/ar/python-net/aspose.cells.drawing/picture)
