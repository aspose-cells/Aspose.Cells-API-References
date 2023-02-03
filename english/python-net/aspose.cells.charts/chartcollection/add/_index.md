---
title: add method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 20
url: /python-net/aspose.cells.charts/chartcollection/add/
is_root: false
---

## add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column) {#ChartType-int-int-int-int}

Adds a chart to the collection.


### Returns 


[Chart](/cells/python-net/aspose.cells.charts/chart) object index.


```python
def add(self, type, upper_left_row, upper_left_column, lower_right_row, lower_right_column):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| type | [ChartType](/cells/python-net/aspose.cells.charts/charttype) | Chart type |
| upper_left_row | int | Upper left row index. |
| upper_left_column | int | Upper left column index. |
| lower_right_row | int | Lower right row index |
| lower_right_column | int | Lower right column index |


## add(type, data_range, top_row, left_column, right_row, bottom_column) {#ChartType-str-int-int-int-int}

Adds a chart to the collection.


### Returns 


[Chart](/cells/python-net/aspose.cells.charts/chart) object index.


```python
def add(self, type, data_range, top_row, left_column, right_row, bottom_column):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| type | [ChartType](/cells/python-net/aspose.cells.charts/charttype) | Chart type |
| data_range | str | Specifies the data range of the chart |
| top_row | int | Upper left row index. |
| left_column | int | Upper left column index. |
| right_row | int | Lower right row index |
| bottom_column | int | Lower right column index |
### Remarks

NOTE: This member is now obsolete. Instead, 
please use [ChartCollection.add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column)](/cells/python-net/aspose.cells.charts/chartcollection/add) property.
This property will be removed 12 months later since May 2022. 
Aspose apologizes for any inconvenience you may have experienced.

## add(data, data_range, is_vertical, top_row, left_column, right_row, bottom_column) {#bytes-str-bool-int-int-int-int}

Adds a chart with preset template.


### Returns 


[Chart](/cells/python-net/aspose.cells.charts/chart) object index.


```python
def add(self, data, data_range, is_vertical, top_row, left_column, right_row, bottom_column):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| data | bytes | The data of chart template file(.crtx). |
| data_range | str | Specifies the data range of the chart |
| is_vertical | bool | Specifies whether to plot the series from a range of cell values by row or by column. |
| top_row | int | Upper left row index. |
| left_column | int | Upper left column index. |
| right_row | int | Lower right row index |
| bottom_column | int | Lower right column index |


## add(type, data_range, is_vertical, top_row, left_column, right_row, bottom_column) {#ChartType-str-bool-int-int-int-int}

Adds a chart to the collection.


### Returns 


[Chart](/cells/python-net/aspose.cells.charts/chart) object index.


```python
def add(self, type, data_range, is_vertical, top_row, left_column, right_row, bottom_column):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| type | [ChartType](/cells/python-net/aspose.cells.charts/charttype) | Chart type |
| data_range | str | Specifies the data range of the chart |
| is_vertical | bool | Specifies whether to plot the series from a range of cell values by row or by column. |
| top_row | int | Upper left row index. |
| left_column | int | Upper left column index. |
| right_row | int | Lower right row index |
| bottom_column | int | Lower right column index |



### See Also
* module [aspose.cells.charts](../../)
* class [ChartCollection](/cells/python-net/aspose.cells.charts/chartcollection)
