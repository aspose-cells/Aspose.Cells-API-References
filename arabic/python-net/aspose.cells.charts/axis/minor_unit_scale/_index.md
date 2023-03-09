---
title: minor_unit_scale الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 360
url: /ar/python-net/aspose.cells.charts/axis/minor_unit_scale/
is_root: false
---
##  minor_unit_scale الملكية

يمثل مقياس الوحدة الرئيسية لمحور الفئة.

###  أمثلة

```python
from aspose.cells.charts import CategoryType, TimeUnit

chart.category_axis.category_type = CategoryType.TIME_SCALE
chart.category_axis.minor_unit_scale = TimeUnit.MONTHS
chart.category_axis.minor_unit = 2

```
###  تعريف:
```python
@property
def minor_unit_scale(self):
    ...
@minor_unit_scale.setter
def minor_unit_scale(self, value):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells.charts](../../)
* فئة [Axis](/cells/ar/python-net/aspose.cells.charts/axis)
* فئة [TimeUnit](/cells/ar/python-net/aspose.cells.charts/timeunit)
