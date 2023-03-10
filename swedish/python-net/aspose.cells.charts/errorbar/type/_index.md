---
title: type fastighet
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 270
url: /sv/python-net/aspose.cells.charts/errorbar/type/
is_root: false
---
##  type fastighet

Representerar felfältsbeloppet type.

###  Exempel

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

###  Se även
* modul [aspose.cells.charts](../../)
* klass [ErrorBar](/cells/sv/python-net/aspose.cells.charts/errorbar)
* klass [ErrorBarType](/cells/sv/python-net/aspose.cells.charts/errorbartype)
