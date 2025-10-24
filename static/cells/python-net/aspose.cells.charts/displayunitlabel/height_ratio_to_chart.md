##height_ratio_to_chart property
## height_ratio_to_chart property
Gets or sets the height of frame in units of ratio of the chart area.
### Remarks
This is a fraction value, its valid range is between 0-1.
How to convert units of ratio to pixels?
HeightPixel = HeightRatioToChart * Chart.ChartObject.Height;
### Definition:
```python
@property
def height_ratio_to_chart(self):
...
@height_ratio_to_chart.setter
def height_ratio_to_chart(self, value):
...
```
### See Also
* module [`aspose.cells.charts`](../../)
* class [`DisplayUnitLabel`](/cells/python-net/aspose.cells.charts/displayunitlabel)
