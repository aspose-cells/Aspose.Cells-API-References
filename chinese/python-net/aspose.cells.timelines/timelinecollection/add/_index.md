---
title: add方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells.timelines/timelinecollection/add/
is_root: false
---
##  add(pivot, dest_cell_name, base_field_name) {#aspose.cells.pivot.PivotTable-str-str}
使用数据透视表作为数据源添加新的时间线


### 返回

新的 add Timeline 索引


```python
def add(self, pivot, dest_cell_name, base_field_name):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |数据透视表对象|
| dest_cell_name | str |时间轴范围左上角的单元格名称。|
| base_field_name | str |PivotTable.BaseFields 中 PivotField 的名称|

### 例子

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i15", "date")

```


##  add(pivot, dest_cell_name, base_field_index) {#aspose.cells.pivot.PivotTable-str-int}
使用数据透视表作为数据源添加新的时间线


### 返回

新的 add Timeline 索引


```python
def add(self, pivot, dest_cell_name, base_field_index):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |数据透视表对象|
| dest_cell_name | str |时间轴范围左上角的单元格名称。|
| base_field_index | int | PivotTable.BaseFields 中 PivotField 的索引|

### 例子

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i5", 1)

```


##  add(pivot, dest_cell_name, base_field) {#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField}
使用数据透视表作为数据源添加新的时间线


### 返回

新的 add Timeline 索引


```python
def add(self, pivot, dest_cell_name, base_field):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |数据透视表对象|
| dest_cell_name | str |时间轴范围左上角的单元格名称。|
| base_field | aspose.cells.pivot.PivotField |PivotTable.BaseFields 中的 PivotField|

### 例子

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, "i10", pivot.base_fields[1])

```


##  add(pivot, row, column, base_field_name) {#aspose.cells.pivot.PivotTable-int-int-str}
使用数据透视表作为数据源添加新的时间线


### 返回

新的 add Timeline 索引


```python
def add(self, pivot, row, column, base_field_name):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |数据透视表对象|
| row | int |时间轴范围左上角单元格的行索引。|
| column | int |时间轴范围左上角单元格的列索引。|
| base_field_name | str |PivotTable.BaseFields 中 PivotField 的名称|

### 例子

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 10, 5, "date")

```


##  add(pivot, row, column, base_field_index) {#aspose.cells.pivot.PivotTable-int-int-int}
使用数据透视表作为数据源添加新的时间线


### 返回

新的 add Timeline 索引


```python
def add(self, pivot, row, column, base_field_index):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |数据透视表对象|
| row | int |时间轴范围左上角单元格的行索引。|
| column | int |时间轴范围左上角单元格的列索引。|
| base_field_index | int | PivotTable.BaseFields 中 PivotField 的索引|

### 例子

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 15, 5, 1)

```


##  add(pivot, row, column, base_field) {#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField}
使用数据透视表作为数据源添加新的时间线


### 返回

新的 add Timeline 索引


```python
def add(self, pivot, row, column, base_field):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |数据透视表对象|
| row | int |时间轴范围左上角单元格的行索引。|
| column | int |时间轴范围左上角单元格的列索引。|
| base_field | aspose.cells.pivot.PivotField |PivotTable.BaseFields 中的 PivotField|

### 例子

```python

# Add a new Timeline using PivotTable as data source
sheet.timelines.add(pivot, 20, 5, pivot.base_fields[1])

```



### 也可以看看
* 模块 [aspose.cells.timelines](../../)
* 类 [TimelineCollection](/cells/zh/python-net/aspose.cells.timelines/timelinecollection)
