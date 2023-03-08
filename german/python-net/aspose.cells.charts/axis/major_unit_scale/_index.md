---
title: major_unit_scale Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 300
url: /de/python-net/aspose.cells.charts/axis/major_unit_scale/
is_root: false
---
##  major_unit_scale Eigentum

Stellt die Haupteinheitsskala für die Kategorieachse dar.

###  Beispiel

```python
from aspose.cells.charts import CategoryType, TimeUnit

chart.category_axis.category_type = CategoryType.TIME_SCALE
chart.category_axis.major_unit_scale = TimeUnit.MONTHS
chart.category_axis.major_unit = 2

```
###  Definition:
```python
@property
def major_unit_scale(self):
    ...
@major_unit_scale.setter
def major_unit_scale(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells.charts](../../)
* Klasse [Axis](/cells/de/python-net/aspose.cells.charts/axis)
* Klasse [TimeUnit](/cells/de/python-net/aspose.cells.charts/timeunit)
