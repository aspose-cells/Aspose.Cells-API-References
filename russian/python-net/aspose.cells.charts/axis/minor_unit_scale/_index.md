---
title: minor_unit_scale недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 360
url: /ru/python-net/aspose.cells.charts/axis/minor_unit_scale/
is_root: false
---
##  minor_unit_scale недвижимость

Представляет шкалу основных единиц для оси категорий.

###  Пример

```python
from aspose.cells.charts import CategoryType, TimeUnit

chart.category_axis.category_type = CategoryType.TIME_SCALE
chart.category_axis.minor_unit_scale = TimeUnit.MONTHS
chart.category_axis.minor_unit = 2

```
###  Определение:
```python
@property
def minor_unit_scale(self):
    ...
@minor_unit_scale.setter
def minor_unit_scale(self, value):
    ...
```

###  Смотрите также
* модуль [aspose.cells.charts](../../)
* класс [Axis](/cells/ru/python-net/aspose.cells.charts/axis)
* класс [TimeUnit](/cells/ru/python-net/aspose.cells.charts/timeunit)
