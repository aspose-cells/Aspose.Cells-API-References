---
title: minor_unit_scale propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 360
url: /fr/python-net/aspose.cells.charts/axis/minor_unit_scale/
is_root: false
---
##  minor_unit_scale propriété

Représente l'échelle des unités principales pour l'axe des abscisses.

###  Exemple

```python
from aspose.cells.charts import CategoryType, TimeUnit

chart.category_axis.category_type = CategoryType.TIME_SCALE
chart.category_axis.minor_unit_scale = TimeUnit.MONTHS
chart.category_axis.minor_unit = 2

```
###  Définition:
```python
@property
def minor_unit_scale(self):
    ...
@minor_unit_scale.setter
def minor_unit_scale(self, value):
    ...
```

###  Voir également
* module [aspose.cells.charts](../../)
* classe [Axis](/cells/fr/python-net/aspose.cells.charts/axis)
* classe [TimeUnit](/cells/fr/python-net/aspose.cells.charts/timeunit)
