---
title: major_unit_scale proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 300
url: /it/python-net/aspose.cells.charts/axis/major_unit_scale/
is_root: false
---
##  major_unit_scale proprietà

Rappresenta la scala dell'unità principale per l'asse delle categorie.

###  Esempio

```python
from aspose.cells.charts import CategoryType, TimeUnit

chart.category_axis.category_type = CategoryType.TIME_SCALE
chart.category_axis.major_unit_scale = TimeUnit.MONTHS
chart.category_axis.major_unit = 2

```
###  Definizione:
```python
@property
def major_unit_scale(self):
    ...
@major_unit_scale.setter
def major_unit_scale(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells.charts](../../)
* classe [Axis](/cells/it/python-net/aspose.cells.charts/axis)
* classe [TimeUnit](/cells/it/python-net/aspose.cells.charts/timeunit)
