---
title: major_unit_scale propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 300
url: /es/python-net/aspose.cells.charts/axis/major_unit_scale/
is_root: false
---
##  major_unit_scale propiedad

Representa la escala de unidad principal para el eje de categorías.

###  Ejemplo

```python
from aspose.cells.charts import CategoryType, TimeUnit

chart.category_axis.category_type = CategoryType.TIME_SCALE
chart.category_axis.major_unit_scale = TimeUnit.MONTHS
chart.category_axis.major_unit = 2

```
###  Definición:
```python
@property
def major_unit_scale(self):
    ...
@major_unit_scale.setter
def major_unit_scale(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells.charts](../../)
* clase [Axis](/cells/es/python-net/aspose.cells.charts/axis)
* clase [TimeUnit](/cells/es/python-net/aspose.cells.charts/timeunit)
