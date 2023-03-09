---
title: minor_unit_scale fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 360
url: /sv/python-net/aspose.cells.charts/axis/minor_unit_scale/
is_root: false
---
##  minor_unit_scale fastighet

Representerar huvudenhetsskalan för kategoriaxeln.

###  Exempel

```python
from aspose.cells.charts import CategoryType, TimeUnit

chart.category_axis.category_type = CategoryType.TIME_SCALE
chart.category_axis.minor_unit_scale = TimeUnit.MONTHS
chart.category_axis.minor_unit = 2

```
###  Definition:
```python
@property
def minor_unit_scale(self):
    ...
@minor_unit_scale.setter
def minor_unit_scale(self, value):
    ...
```

###  Se även
* modul [aspose.cells.charts](../../)
* klass [Axis](/cells/sv/python-net/aspose.cells.charts/axis)
* klass [TimeUnit](/cells/sv/python-net/aspose.cells.charts/timeunit)
