##inner_height_ratio_to_chart property
## inner_height_ratio_to_chart property
Gets or sets the height of plot area in units of ratio of the chart area.
### Remarks
The plot-area bounding box includes the plot area, tick marks(tick labels), and a small border around the tick marks.
If the value is not created by MS Excel, please call Chart.Calculate() method before calling this method.
The **XRatioToChart** , **YRatioToChart** , **WidthRatioToChart**  and **HeightRatioToChart**  of **PlotArea**  represents the plot-area
bounding box that includes the plot area, tick marks(tick labels), and a small border around the tick marks.
If you want to get actual size of plot area, you should call **InnerXRatioToChart** , **InnerYRatioToChart** , **InnerWidthRatioToChart**  and
**InnerHeightRatioToChart**  properties.
For excel 2007 or latter, the default value is zero. you should call get the value after calling Chart.Calculate().
InnerHeight in Pixel = InnerXRatioToChart * chart.ChartObject.Width.
### Definition:
```python
@property
def inner_height_ratio_to_chart(self):
...
@inner_height_ratio_to_chart.setter
def inner_height_ratio_to_chart(self, value):
...
```
### See Also
* module [`aspose.cells.charts`](../../)
* class [`PlotArea`](/cells/python-net/aspose.cells.charts/plotarea)
