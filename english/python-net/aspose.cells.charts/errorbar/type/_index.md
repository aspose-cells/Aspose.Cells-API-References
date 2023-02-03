---
title: type property
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 270
url: /python-net/aspose.cells.charts/errorbar/type/
is_root: false
---

## type property


Represents error bar amount type.

### Example 


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

### See Also
* module [aspose.cells.charts](../../)
* class [ErrorBar](/cells/python-net/aspose.cells.charts/errorbar)
