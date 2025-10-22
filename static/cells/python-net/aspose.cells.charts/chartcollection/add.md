##add method
## add(self, type, upper_left_row, upper_left_column, lower_right_row, lower_right_column) {#aspose.cells.charts.ChartType-int-int-int-int}
Adds a chart to the collection.
### Returns
[`Chart`](/cells/python-net/aspose.cells.charts/chart) object index.
```python
def add(self, type, upper_left_row, upper_left_column, lower_right_row, lower_right_column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| type | aspose.cells.charts.ChartType | Chart type |
| upper_left_row | int | Upper left row index. |
| upper_left_column | int | Upper left column index. |
| lower_right_row | int | Lower right row index |
| lower_right_column | int | Lower right column index |
## add(self, type, data_range, top_row, left_column, right_row, bottom_column) {#aspose.cells.charts.ChartType-System.String-int-int-int-int}
Adds a chart to the collection.
### Returns
[`Chart`](/cells/python-net/aspose.cells.charts/chart) object index.
```python
def add(self, type, data_range, top_row, left_column, right_row, bottom_column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| type | aspose.cells.charts.ChartType | Chart type |
| data_range | System.String | Specifies the data range of the chart |
| top_row | int | Upper left row index. |
| left_column | int | Upper left column index. |
| right_row | int | Lower right row index |
| bottom_column | int | Lower right column index |
### Remarks
NOTE: This member is now obsolete. Instead,
please use [`ChartCollection.add`](/cells/python-net/aspose.cells.charts/chartcollection/add) property.
This property will be removed 12 months later since May 2022.
Aspose apologizes for any inconvenience you may have experienced.
## add(self, data, data_range, is_vertical, top_row, left_column, right_row, bottom_column) {#bytes-System.String-bool-int-int-int-int}
Adds a chart with preset template.
### Returns
[`Chart`](/cells/python-net/aspose.cells.charts/chart) object index.
```python
def add(self, data, data_range, is_vertical, top_row, left_column, right_row, bottom_column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| data | bytes | The data of chart template file(.crtx). |
| data_range | System.String | Specifies the data range of the chart |
| is_vertical | bool | Specifies whether to plot the series from a range of cell values by row or by column. |
| top_row | int | Upper left row index. |
| left_column | int | Upper left column index. |
| right_row | int | Lower right row index |
| bottom_column | int | Lower right column index |
## add(self, type, data_range, is_vertical, top_row, left_column, right_row, bottom_column) {#aspose.cells.charts.ChartType-System.String-bool-int-int-int-int}
Adds a chart to the collection.
### Returns
[`Chart`](/cells/python-net/aspose.cells.charts/chart) object index.
```python
def add(self, type, data_range, is_vertical, top_row, left_column, right_row, bottom_column):
...
```
| Parameter | Type | Description |
| :- | :- | :- |
| type | aspose.cells.charts.ChartType | Chart type |
| data_range | System.String | Specifies the data range of the chart |
| is_vertical | bool | Specifies whether to plot the series from a range of cell values by row or by column. |
| top_row | int | Upper left row index. |
| left_column | int | Upper left column index. |
| right_row | int | Lower right row index |
| bottom_column | int | Lower right column index |
### See Also
* module [`aspose.cells.charts`](../../)
* class [`Chart`](/cells/python-net/aspose.cells.charts/chart)
* class [`ChartCollection`](/cells/python-net/aspose.cells.charts/chartcollection)
