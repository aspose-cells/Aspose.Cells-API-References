---
title: add方法
second_title: Aspose.Cells for Python via .NET API 参考文献
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells.slicers/slicercollection/add/
is_root: false
---
##  add(pivot, dest_cell_name, base_field_name) {#aspose.cells.pivot.PivotTable-str-str}
使用数据透视表作为数据源添加新的切片器


### 返回

新的 add 切片器索引


```python
def add(self, pivot, dest_cell_name, base_field_name):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |数据透视表对象|
| dest_cell_name | str |切片器范围左上角的单元格。|
| base_field_name | str | PivotTable.BaseFields 中 PivotField 的名称|

### 例子

```python

slicers.add(pivot, "E3", "fruit")

```


##  add(pivot, dest_cell_name, base_field_index) {#aspose.cells.pivot.PivotTable-str-int}
使用数据透视表作为数据源添加新的切片器


### 返回

新的 add 切片器索引


```python
def add(self, pivot, dest_cell_name, base_field_index):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |数据透视表对象|
| dest_cell_name | str |切片器范围左上角的单元格。|
| base_field_index | int |PivotTable.BaseFields 中 PivotField 的索引|

### 例子

```python

slicers.add(pivot, "E20", 0)

```


##  add(pivot, dest_cell_name, base_field) {#aspose.cells.pivot.PivotTable-str-aspose.cells.pivot.PivotField}
使用数据透视表作为数据源添加新的切片器


### 返回

新的 add 切片器索引


```python
def add(self, pivot, dest_cell_name, base_field):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |数据透视表对象|
| dest_cell_name | str |切片器范围左上角的单元格。|
| base_field | aspose.cells.pivot.PivotField |PivotTable.BaseFields 中的 PivotField|

### 例子

```python

slicers.add(pivot, "I3", pivot.base_fields[0])

```


##  add(table, index, dest_cell_name) {#aspose.cells.tables.ListObject-int-str}
使用 ListObjet 作为数据源添加一个新的切片器


### 返回

新的 add 切片器索引


```python
def add(self, table, index, dest_cell_name):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| table | aspose.cells.tables.ListObject |ListObject 对象|
| index | int |ListObject.ListColumns 中 ListColumn 的索引|
| dest_cell_name | str |切片器范围左上角的单元格。|

### 例子

```python

slicers.add(table, 1, "E38")

```


##  add(table, list_column, dest_cell_name) {#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-str}
使用 ListObjet 作为数据源添加一个新的切片器


### 返回

新的 add 切片器索引


```python
def add(self, table, list_column, dest_cell_name):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| table | aspose.cells.tables.ListObject |ListObject 对象|
| list_column | aspose.cells.tables.ListColumn |ListObject.ListColumns 中的 ListColumn|
| dest_cell_name | str |切片器范围左上角的单元格。|

### 例子

```python

slicers.add(table, table.list_columns[1], "I38")

```


##  add(pivot, row, column, base_field_name) {#aspose.cells.pivot.PivotTable-int-int-str}
使用数据透视表作为数据源添加新的切片器


### 返回

新的 add 切片器索引


```python
def add(self, pivot, row, column, base_field_name):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |数据透视表对象|
| row | int |切片器范围左上角单元格的行索引。|
| column | int |切片器区域左上角单元格的列索引。|
| base_field_name | str | PivotTable.BaseFields 中 PivotField 的名称|

### 例子

```python

slicers.add(pivot, 20, 12, "fruit")

```


##  add(pivot, row, column, base_field_index) {#aspose.cells.pivot.PivotTable-int-int-int}
使用数据透视表作为数据源添加新的切片器


### 返回

新的 add 切片器索引


```python
def add(self, pivot, row, column, base_field_index):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |数据透视表对象|
| row | int |切片器范围左上角单元格的行索引。|
| column | int |切片器区域左上角单元格的列索引。|
| base_field_index | int |PivotTable.BaseFields 中 PivotField 的索引|

### 例子

```python

slicers.add(pivot, 20, 8, 0)

```


##  add(pivot, row, column, base_field) {#aspose.cells.pivot.PivotTable-int-int-aspose.cells.pivot.PivotField}
使用数据透视表作为数据源添加新的切片器


### 返回

新的 add 切片器索引


```python
def add(self, pivot, row, column, base_field):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| pivot | aspose.cells.pivot.PivotTable |数据透视表对象|
| row | int |切片器范围左上角单元格的行索引。|
| column | int |切片器区域左上角单元格的列索引。|
| base_field | aspose.cells.pivot.PivotField |PivotTable.BaseFields 中的 PivotField|

### 例子

```python

slicers.add(pivot, 3, 12, pivot.base_fields[0])

```


##  add(table, list_column, row, column) {#aspose.cells.tables.ListObject-aspose.cells.tables.ListColumn-int-int}
使用 ListObjet 作为数据源添加一个新的切片器


### 返回

新的 add 切片器索引


```python
def add(self, table, list_column, row, column):
    ...
```


|参数|类型|描述|
| :- | :- | :- |
| table | aspose.cells.tables.ListObject |ListObject 对象|
| list_column | aspose.cells.tables.ListColumn |ListObject.ListColumns 中的 ListColumn|
| row | int |切片器范围左上角单元格的行索引。|
| column | int |切片器区域左上角单元格的列索引。|

### 例子

```python

slicers.add(table, table.list_columns[1], 38, 12)

```



### 也可以看看
* 模块 [aspose.cells.slicers](../../)
* 类 [SlicerCollection](/cells/zh/python-net/aspose.cells.slicers/slicercollection)
