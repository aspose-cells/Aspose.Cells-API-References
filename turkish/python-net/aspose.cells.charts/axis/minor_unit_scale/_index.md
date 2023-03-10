---
title: minor_unit_scale mülk
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 360
url: /tr/python-net/aspose.cells.charts/axis/minor_unit_scale/
is_root: false
---
##  minor_unit_scale mülk

Kategori ekseni için ana birim ölçeğini temsil eder.

###  Örnek

```python
from aspose.cells.charts import CategoryType, TimeUnit

chart.category_axis.category_type = CategoryType.TIME_SCALE
chart.category_axis.minor_unit_scale = TimeUnit.MONTHS
chart.category_axis.minor_unit = 2

```
###  Tanım:
```python
@property
def minor_unit_scale(self):
    ...
@minor_unit_scale.setter
def minor_unit_scale(self, value):
    ...
```

###  Ayrıca bakınız
* modül [aspose.cells.charts](../../)
* sınıf [Axis](/cells/tr/python-net/aspose.cells.charts/axis)
* sınıf [TimeUnit](/cells/tr/python-net/aspose.cells.charts/timeunit)
