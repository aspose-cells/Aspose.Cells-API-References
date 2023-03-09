---
title: type недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 270
url: /ru/python-net/aspose.cells.charts/errorbar/type/
is_root: false
---
##  type недвижимость

Представляет количество ошибок type.

###  Пример

```python
from aspose.cells import Workbook
from aspose.cells.charts import ErrorBarType

wb = Workbook("chart.xlsx")
chart = wb.worksheets[0].charts[0]
aseries = chart.n_series[0]
# Sets custom error bar type
aseries.y_error_bar.type = ErrorBarType.CUSTOM
aseries.y_error_bar.plus_value = "=Sheet1!A1"
aseries.y_error_bar.minus_value = "=Sheet1!A2"

```
###  Определение:
```python
@property
def type(self):
    ...
@type.setter
def type(self, value):
    ...
```

###  Смотрите также
* модуль [aspose.cells.charts](../../)
* класс [ErrorBar](/cells/ru/python-net/aspose.cells.charts/errorbar)
* класс [ErrorBarType](/cells/ru/python-net/aspose.cells.charts/errorbartype)
