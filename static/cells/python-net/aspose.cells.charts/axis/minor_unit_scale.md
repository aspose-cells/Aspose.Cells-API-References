##minor_unit_scale property
## minor_unit_scale property
Represents the major unit scale for the category axis.
### Example
```python
from aspose.cells.charts import CategoryType, TimeUnit
chart.category_axis.category_type = CategoryType.TIME_SCALE
chart.category_axis.minor_unit_scale = TimeUnit.MONTHS
chart.category_axis.minor_unit = 2.0
```
### Definition:
```python
@property
def minor_unit_scale(self):
...
@minor_unit_scale.setter
def minor_unit_scale(self, value):
...
```
### See Also
* module [`aspose.cells.charts`](../../)
* class [`Axis`](/cells/python-net/aspose.cells.charts/axis)
* class [`TimeUnit`](/cells/python-net/aspose.cells.charts/timeunit)
