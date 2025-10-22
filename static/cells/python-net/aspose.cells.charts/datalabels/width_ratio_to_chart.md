##width_ratio_to_chart property
## width_ratio_to_chart property
Gets or sets the width of frame in units of ratio of the chart area.
### Remarks
This is a fraction value, its valid range is between 0-1.
How to convert units of ratio to pixels?
WidthPixel = WidthRatioToChart * Chart.ChartObject.Width;
### Definition:
```python
@property
def width_ratio_to_chart(self):
...
@width_ratio_to_chart.setter
def width_ratio_to_chart(self, value):
...
```
### See Also
* module [`aspose.cells.charts`](../../)
* class [`DataLabels`](/cells/python-net/aspose.cells.charts/datalabels)
