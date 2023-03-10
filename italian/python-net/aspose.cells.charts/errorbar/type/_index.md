---
title: type proprietà
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 270
url: /it/python-net/aspose.cells.charts/errorbar/type/
is_root: false
---
##  type proprietà

Rappresenta l'importo della barra di errore type.

###  Esempio

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
###  Definizione:
```python
@property
def type(self):
    ...
@type.setter
def type(self, value):
    ...
```

###  Guarda anche
* modulo [aspose.cells.charts](../../)
* classe [ErrorBar](/cells/it/python-net/aspose.cells.charts/errorbar)
* classe [ErrorBarType](/cells/it/python-net/aspose.cells.charts/errorbartype)
