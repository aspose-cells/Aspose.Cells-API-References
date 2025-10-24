##ChartPointCollection class
## ChartPointCollection class
Represents a collection that contains all the points in one series.
The ChartPointCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [count](/cells/python-net/aspose.cells.charts/chartpointcollection/count) | Gets the count of the chart point. |
Gets the [`ChartPoint`](/cells/python-net/aspose.cells.charts/chartpoint) element at the specified index in the series.
### Indexer
| Name | Description |
| :- | :- |
| [index] | The index of chart point in the series. |
### Methods
| Method | Description |
| :- | :- |
| [`clear(self)`](/cells/python-net/aspose.cells.charts/chartpointcollection/clear/#) | Remove all setting of the chart points. |
| [`remove_at(self, index)`](/cells/python-net/aspose.cells.charts/chartpointcollection/remove_at/#int) | Removes point at the index of the series.. |
### Example
```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType
from aspose.pydrawing import Color
# Instantiating a Workbook object
workbook = Workbook()
# Obtaining the reference of the first worksheet
worksheet = workbook.worksheets[0]
# Adding a sample value to "A1" cell
worksheet.cells.get("A1").put_value(50)
# Adding a sample value to "A2" cell
worksheet.cells.get("A2").put_value(100)
# Adding a sample value to "A3" cell
worksheet.cells.get("A3").put_value(150)
# Adding a sample value to "B1" cell
worksheet.cells.get("B1").put_value(60)
# Adding a sample value to "B2" cell
worksheet.cells.get("B2").put_value(32)
# Adding a sample value to "B3" cell
worksheet.cells.get("B3").put_value(50)
# Adding a chart to the worksheet
chartIndex = worksheet.charts.add(ChartType.PIE_EXPLODED, 5, 0, 25, 10)
# Accessing the instance of the newly added chart
chart = worksheet.charts[chartIndex]
# Adding NSeries (chart data source) to the chart ranging from "A1" cell to "B3"
chart.n_series.add("A1:B3", True)
# Show Data Labels
chart.n_series[0].data_labels.show_value = True
points = chart.n_series[0].points
for i in range(points.count):
# Get Data Point
point = points[i]
# Set Pir Explosion
point.explosion = 15
# Set Border Color
point.border.color = Color.red
# Saving the Excel file
workbook.save("book1.xls")
```
### See Also
* module [`aspose.cells.charts`](..)
* class [`ChartPoint`](/cells/python-net/aspose.cells.charts/chartpoint)
