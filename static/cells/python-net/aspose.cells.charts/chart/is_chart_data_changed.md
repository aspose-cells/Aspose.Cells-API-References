##is_chart_data_changed method
## is_chart_data_changed(self) {#}
Detects if a chart's data source has changed.
### Returns
Returns true if the chart has changed otherwise returns false
```python
def is_chart_data_changed(self):
...
```
### Remarks
The method detects the changes in the chart's data source before rendering the chart to image format.
At first Chart.toImage call, the chart source data (e.g. XValuesParseData, ValuesParseData) will be recorded.
Before calling the Chart.toImage method again, call IsChartDataChanged method to check if Chart needs re-rendering.
### See Also
* module [`aspose.cells.charts`](../../)
* class [`Chart`](/cells/python-net/aspose.cells.charts/chart)
