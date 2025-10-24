##TrendlineCollection class
## TrendlineCollection class
Represents a collection of all the [`Trendline`](/cells/python-net/aspose.cells.charts/trendline) objects for the specified data series.
The TrendlineCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells.charts/trendlinecollection/capacity) | Gets or sets the number of elements that the array list can contain. |
### Methods
| Method | Description |
| :- | :- |
| [`add(self, type)`](/cells/python-net/aspose.cells.charts/trendlinecollection/add/#aspose.cells.charts.trendlinetype) | Adds a [`Trendline`](/cells/python-net/aspose.cells.charts/trendline) object to this collection with specified type. |
| [`add(self, type, name)`](/cells/python-net/aspose.cells.charts/trendlinecollection/add/#aspose.cells.charts.trendlinetype-system.string) | Adds a [`Trendline`](/cells/python-net/aspose.cells.charts/trendline) object to this collection with specified type and name. |
| [`copy_to(self, array)`](/cells/python-net/aspose.cells.charts/trendlinecollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [`copy_to(self, index, array, array_index, count)`](/cells/python-net/aspose.cells.charts/trendlinecollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [`index_of(self, item, index)`](/cells/python-net/aspose.cells.charts/trendlinecollection/index_of/#aspose.cells.charts.trendline-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [`index_of(self, item, index, count)`](/cells/python-net/aspose.cells.charts/trendlinecollection/index_of/#aspose.cells.charts.trendline-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [`last_index_of(self, item)`](/cells/python-net/aspose.cells.charts/trendlinecollection/last_index_of/#aspose.cells.charts.trendline) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [`last_index_of(self, item, index)`](/cells/python-net/aspose.cells.charts/trendlinecollection/last_index_of/#aspose.cells.charts.trendline-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [`last_index_of(self, item, index, count)`](/cells/python-net/aspose.cells.charts/trendlinecollection/last_index_of/#aspose.cells.charts.trendline-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [`binary_search(self, item)`](/cells/python-net/aspose.cells.charts/trendlinecollection/binary_search/#aspose.cells.charts.trendline) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |
### Example
```python
from aspose.cells import Workbook
from aspose.cells.charts import ChartType, TrendlineType
from aspose.pydrawing import Color
# Instantiating a Workbook object
workbook = Workbook()
# Adding a new worksheet to the Excel object
sheetIndex = workbook.worksheets.add()
# Obtaining the reference of the newly added worksheet by passing its sheet index
worksheet = workbook.worksheets[sheetIndex]
worksheet.cells.get("A1").put_value(50)
worksheet.cells.get("A2").put_value(100)
worksheet.cells.get("A3").put_value(150)
worksheet.cells.get("A4").put_value(200)
worksheet.cells.get("B1").put_value(60)
worksheet.cells.get("B2").put_value(32)
worksheet.cells.get("B3").put_value(50)
worksheet.cells.get("B4").put_value(40)
# Adding a chart to the worksheet
chartIndex = workbook.worksheets[0].charts.add(ChartType.COLUMN, 3, 3, 15, 10)
chart = workbook.worksheets[0].charts[chartIndex]
chart.n_series.add("A1:a3", True)
chart.n_series[0].trend_lines.add(TrendlineType.LINEAR, "MyTrendLine")
line = chart.n_series[0].trend_lines[0]
line.display_equation = True
line.display_r_squared = True
line.color = Color.red
```
### See Also
* module [`aspose.cells.charts`](..)
* class [`Trendline`](/cells/python-net/aspose.cells.charts/trendline)
