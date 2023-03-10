---
title: type الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 270
url: /ar/python-net/aspose.cells.charts/errorbar/type/
is_root: false
---
##  type الملكية

يمثل مقدار شريط الخطأ type.

###  مثال

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
###  تعريف:
```python
@property
def type(self):
    ...
@type.setter
def type(self, value):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells.charts](../../)
* فئة [ErrorBar](/cells/ar/python-net/aspose.cells.charts/errorbar)
* فئة [ErrorBarType](/cells/ar/python-net/aspose.cells.charts/errorbartype)
