##type property
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
### Definition:
```python
@property
def type(self):
...
@type.setter
def type(self, value):
...
```
### See Also
* module [`aspose.cells.charts`](../../)
* class [`ErrorBar`](/cells/python-net/aspose.cells.charts/errorbar)
* class [`ErrorBarType`](/cells/python-net/aspose.cells.charts/errorbartype)
