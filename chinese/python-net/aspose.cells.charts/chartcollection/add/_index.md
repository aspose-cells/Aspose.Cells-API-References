---
title: add方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells.charts/chartcollection/add/
is_root: false
---
##  add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column) {#ChartType-int-int-int-int}
向集合中添加图表。


### 返回

[Chart](/cells/zh/python-net/aspose.cells.charts/chart) 对象索引。


```python
def add(self, type, upper_left_row, upper_left_column, lower_right_row, lower_right_column):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| type | [ChartType](/cells/zh/python-net/aspose.cells.charts/charttype) |图表类型|
| upper_left_row | int |左上行索引。|
| upper_left_column | int |左上列索引。|
| lower_right_row | int |右下行索引|
| lower_right_column | int |右下栏索引|


##  add(type, data_range, top_row, left_column, right_row, bottom_column) {#ChartType-str-int-int-int-int}
向集合中添加图表。


### 返回

[Chart](/cells/zh/python-net/aspose.cells.charts/chart) 对象索引。


```python
def add(self, type, data_range, top_row, left_column, right_row, bottom_column):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| type | [ChartType](/cells/zh/python-net/aspose.cells.charts/charttype) |图表类型|
| data_range | str |指定图表的数据范围|
| top_row | int |左上行索引。|
| left_column | int |左上列索引。|
| right_row | int |右下行索引|
| bottom_column | int |右下栏索引|
### 评论

注意：该成员现已过时。反而，
请使用 [ChartCollection.add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column)](/cells/zh/python-net/aspose.cells.charts/chartcollection/add) 属性。
自 2022 年 5 月起，此属性将在 12 个月后移除。
Aspose 对您可能遇到的任何不便深表歉意。

##  add(data, data_range, is_vertical, top_row, left_column, right_row, bottom_column) {#bytes-str-bool-int-int-int-int}
添加带有预设模板的图表。


### 返回

[Chart](/cells/zh/python-net/aspose.cells.charts/chart) 对象索引。


```python
def add(self, data, data_range, is_vertical, top_row, left_column, right_row, bottom_column):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| data | bytes |图表模板文件（.crtx）的数据。|
| data_range | str |指定图表的数据范围|
| is_vertical | bool |指定是按行还是按列绘制一系列单元格值。|
| top_row | int |左上行索引。|
| left_column | int |左上列索引。|
| right_row | int |右下行索引|
| bottom_column | int |右下栏索引|


##  add(type, data_range, is_vertical, top_row, left_column, right_row, bottom_column) {#ChartType-str-bool-int-int-int-int}
向集合中添加图表。


### 返回

[Chart](/cells/zh/python-net/aspose.cells.charts/chart) 对象索引。


```python
def add(self, type, data_range, is_vertical, top_row, left_column, right_row, bottom_column):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| type | [ChartType](/cells/zh/python-net/aspose.cells.charts/charttype) |图表类型|
| data_range | str |指定图表的数据范围|
| is_vertical | bool |指定是按行还是按列绘制一系列单元格值。|
| top_row | int |左上行索引。|
| left_column | int |左上列索引。|
| right_row | int |右下行索引|
| bottom_column | int |右下栏索引|



### 也可以看看
* 模块 [aspose.cells.charts](../../)
* 类 [Chart](/cells/zh/python-net/aspose.cells.charts/chart)
* 类 [ChartCollection](/cells/zh/python-net/aspose.cells.charts/chartcollection)
