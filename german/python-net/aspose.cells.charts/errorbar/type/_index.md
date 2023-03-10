---
title: type Eigentum
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 270
url: /de/python-net/aspose.cells.charts/errorbar/type/
is_root: false
---
##  type Eigentum

Stellt den Fehlerbalkenbetrag type dar.

###  Beispiel

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
###  Definition:
```python
@property
def type(self):
    ...
@type.setter
def type(self, value):
    ...
```

###  Siehe auch
* Modul [aspose.cells.charts](../../)
* Klasse [ErrorBar](/cells/de/python-net/aspose.cells.charts/errorbar)
* Klasse [ErrorBarType](/cells/de/python-net/aspose.cells.charts/errorbartype)
