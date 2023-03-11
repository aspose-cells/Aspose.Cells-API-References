---
title: type propriété
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 270
url: /fr/python-net/aspose.cells.charts/errorbar/type/
is_root: false
---
##  type propriété

Représente le montant de la barre d'erreur type.

###  Exemple

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
###  Définition:
```python
@property
def type(self):
    ...
@type.setter
def type(self, value):
    ...
```

###  Voir également
* module [aspose.cells.charts](../../)
* classe [ErrorBar](/cells/fr/python-net/aspose.cells.charts/errorbar)
* classe [ErrorBarType](/cells/fr/python-net/aspose.cells.charts/errorbartype)
