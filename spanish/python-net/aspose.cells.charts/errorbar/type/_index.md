---
title: type propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 270
url: /es/python-net/aspose.cells.charts/errorbar/type/
is_root: false
---
##  type propiedad

Representa la cantidad de barra de error type.

###  Ejemplo

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
###  Definición:
```python
@property
def type(self):
    ...
@type.setter
def type(self, value):
    ...
```

###  Ver también
* módulo [aspose.cells.charts](../../)
* clase [ErrorBar](/cells/es/python-net/aspose.cells.charts/errorbar)
* clase [ErrorBarType](/cells/es/python-net/aspose.cells.charts/errorbartype)
