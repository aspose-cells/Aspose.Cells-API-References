##update_all_points property
## update_all_points property
Whether update all data points when performing the chart calculation. Default: False.
When you want to get the value for each data point in the chart specifically, set it to true.
If this parameter is set to True, the new data points may be generated when chart is calculated. This could make the Excel file larger.
### Definition:
```python
@property
def update_all_points(self):
...
@update_all_points.setter
def update_all_points(self, value):
...
```
### See Also
* module [`aspose.cells.charts`](../../)
* class [`ChartCalculateOptions`](/cells/python-net/aspose.cells.charts/chartcalculateoptions)
