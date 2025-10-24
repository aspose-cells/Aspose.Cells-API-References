##ChartCollection class
## ChartCollection class
Encapsulates a collection of [`Chart`](/cells/python-net/aspose.cells.charts/chart) objects.
The ChartCollection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [capacity](/cells/python-net/aspose.cells.charts/chartcollection/capacity) | Gets or sets the number of elements that the array list can contain. |
### Methods
| Method | Description |
| :- | :- |
| [`add(self, type, upper_left_row, upper_left_column, lower_right_row, lower_right_column)`](/cells/python-net/aspose.cells.charts/chartcollection/add/#aspose.cells.charts.charttype-int-int-int-int) | Adds a chart to the collection. |
| [`add(self, type, data_range, top_row, left_column, right_row, bottom_column)`](/cells/python-net/aspose.cells.charts/chartcollection/add/#aspose.cells.charts.charttype-system.string-int-int-int-int) | Adds a chart to the collection. |
| [`add(self, data, data_range, is_vertical, top_row, left_column, right_row, bottom_column)`](/cells/python-net/aspose.cells.charts/chartcollection/add/#bytes-system.string-bool-int-int-int-int) | Adds a chart with preset template. |
| [`add(self, type, data_range, is_vertical, top_row, left_column, right_row, bottom_column)`](/cells/python-net/aspose.cells.charts/chartcollection/add/#aspose.cells.charts.charttype-system.string-bool-int-int-int-int) | Adds a chart to the collection. |
| [`get(self, index)`](/cells/python-net/aspose.cells.charts/chartcollection/get/#int) | Add API for Python Via .Net.since this[int index] is unsupported |
| [`get(self, name)`](/cells/python-net/aspose.cells.charts/chartcollection/get/#system.string) | Add API for Python Via .Net.since this[string Chart] is unsupported |
| [`copy_to(self, array)`](/cells/python-net/aspose.cells.charts/chartcollection/copy_to/#list) | Copies the entire array list to a compatible one-dimensional array list, starting at the beginning of the target array list. |
| [`copy_to(self, index, array, array_index, count)`](/cells/python-net/aspose.cells.charts/chartcollection/copy_to/#int-list-int-int) | Copies a range of elements from the array list to a compatible one-dimensional array list, starting at the specified index of the target array list. |
| [`index_of(self, item, index)`](/cells/python-net/aspose.cells.charts/chartcollection/index_of/#aspose.cells.charts.chart-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that extends from the specified index to the last element. |
| [`index_of(self, item, index, count)`](/cells/python-net/aspose.cells.charts/chartcollection/index_of/#aspose.cells.charts.chart-int-int) | Searches for the specified object and returns the zero-based index of the first occurrence within the range of elements in the array list that starts at the specified index and contains the specified number of elements. |
| [`last_index_of(self, item)`](/cells/python-net/aspose.cells.charts/chartcollection/last_index_of/#aspose.cells.charts.chart) | Searches for the specified object and returns the zero-based index of the last occurrence within the entire array list. |
| [`last_index_of(self, item, index)`](/cells/python-net/aspose.cells.charts/chartcollection/last_index_of/#aspose.cells.charts.chart-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that extends from the first element to the specified index. |
| [`last_index_of(self, item, index, count)`](/cells/python-net/aspose.cells.charts/chartcollection/last_index_of/#aspose.cells.charts.chart-int-int) | Searches for the specified object and returns the zero-based index of the last occurrence within the range of elements in the array list that contains the specified number of elements and ends at the specified index. |
| [`add_floating_chart(self, type, left, top, width, height)`](/cells/python-net/aspose.cells.charts/chartcollection/add_floating_chart/#aspose.cells.charts.charttype-int-int-int-int) | Adds a chart to the collection. |
| [`binary_search(self, item)`](/cells/python-net/aspose.cells.charts/chartcollection/binary_search/#aspose.cells.charts.chart) | Searches the entire sorted array list for an element using the default comparer and returns the zero-based index of the element. |
### Example
```python
from aspose.cells import Workbook
workbook = Workbook()
charts = workbook.worksheets[0].charts
```
### See Also
* module [`aspose.cells.charts`](..)
* class [`Chart`](/cells/python-net/aspose.cells.charts/chart)
