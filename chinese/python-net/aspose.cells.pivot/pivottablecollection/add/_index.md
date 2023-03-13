---
title: add方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 20
url: /zh/python-net/aspose.cells.pivot/pivottablecollection/add/
is_root: false
---
##  add(source_data, dest_cell_name, table_name) {#str-str-str}
将新的数据透视表缓存添加到 PivotCaches 集合。


### 返回

新添加的缓存索引。


```python
def add(self, source_data, dest_cell_name, table_name):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| source_data | str |新数据透视表缓存的数据。|
| dest_cell_name | str |数据透视表目标区域左上角的单元格。|
| table_name | str |新数据透视表的名称。|


##  add(pivot_table, dest_cell_name, table_name) {#PivotTable-str-str}
将新的数据透视表对象添加到另一个数据透视表的集合中。


### 返回

新添加的数据透视表索引。


```python
def add(self, pivot_table, dest_cell_name, table_name):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| pivot_table | [PivotTable](/cells/zh/python-net/aspose.cells.pivot/pivottable) |源数据透视表。|
| dest_cell_name | str |数据透视表目标区域左上角的单元格。|
| table_name | str |新数据透视表的名称。|


##  add(source_data, dest_cell_name, table_name, use_same_source) {#str-str-str-bool}
将新的数据透视表缓存添加到 PivotCaches 集合。


### 返回

新添加的缓存索引。


```python
def add(self, source_data, dest_cell_name, table_name, use_same_source):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| source_data | str |新数据透视表缓存的数据。|
| dest_cell_name | str |数据透视表目标区域左上角的单元格。|
| table_name | str |新数据透视表的名称。|
| use_same_source | bool |指示当另一个现有数据透视表已使用此数据源时是否使用相同的数据源。<br/>如果该属性为真，它将节省内存。|


##  add(source_data, row, column, table_name) {#str-int-int-str}
将新的数据透视表缓存添加到 PivotCaches 集合。


### 返回

新添加的缓存索引。


```python
def add(self, source_data, row, column, table_name):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| source_data | str |新数据透视表的数据单元格范围。示例：Sheet1!A1:C8|
| row | int |数据透视表目标区域左上角单元格的行索引。|
| column | int |数据透视表目标区域左上角单元格的列索引。|
| table_name | str |新数据透视表的名称。|


##  add(pivot_table, row, column, table_name) {#PivotTable-int-int-str}
将新的数据透视表对象添加到另一个数据透视表的集合中。


### 返回

新添加的数据透视表索引。


```python
def add(self, pivot_table, row, column, table_name):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| pivot_table | [PivotTable](/cells/zh/python-net/aspose.cells.pivot/pivottable) |源数据透视表。|
| row | int |数据透视表目标区域左上角单元格的行索引。|
| column | int |数据透视表目标区域左上角单元格的列索引。|
| table_name | str |新数据透视表的名称。|


##  add(source_data, row, column, table_name, use_same_source) {#str-int-int-str-bool}
将新的数据透视表缓存添加到 PivotCaches 集合。


### 返回

新添加的缓存索引。


```python
def add(self, source_data, row, column, table_name, use_same_source):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| source_data | str |新数据透视表的数据单元格范围。示例：Sheet1!A1:C8|
| row | int |数据透视表目标区域左上角单元格的行索引。|
| column | int |数据透视表目标区域左上角单元格的列索引。|
| table_name | str |新数据透视表的名称。|
| use_same_source | bool |指示当另一个现有数据透视表已使用此数据源时是否使用相同的数据源。<br/>如果该属性为真，它将节省内存。|


##  add(source_data, is_auto_page, page_fields, dest_cell_name, table_name) {#list-bool-PivotPageFields-str-str}
将新的数据透视表对象添加到具有多个合并范围作为数据源的集合中。


### 返回

新添加的数据透视表索引。


```python
def add(self, source_data, is_auto_page, page_fields, dest_cell_name, table_name):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| source_data | list |多个合并范围，如{"Sheet1!A1:C8","Sheet2!A1:B8"} |
| is_auto_page | bool |是否自动创建单页字段。<br/>如果为真，后面的参数 pageFields 将被忽略。|
| page_fields | [PivotPageFields](/cells/zh/python-net/aspose.cells.pivot/pivotpagefields) |数据透视页字段项。|
| dest_cell_name | str | destCellName 新数据透视表的名称。|
| table_name | str |新数据透视表的名称。|


##  add(source_data, is_auto_page, page_fields, row, column, table_name) {#list-bool-PivotPageFields-int-int-str}
将新的数据透视表对象添加到具有多个合并范围作为数据源的集合中。


### 返回

新添加的数据透视表索引。


```python
def add(self, source_data, is_auto_page, page_fields, row, column, table_name):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| source_data | list |多个合并范围，如{"Sheet1!A1:C8","Sheet2!A1:B8"} |
| is_auto_page | bool |是否自动创建单页字段。<br/>如果为真，后面的参数 pageFields 将被忽略|
| page_fields | [PivotPageFields](/cells/zh/python-net/aspose.cells.pivot/pivotpagefields) |数据透视页字段项。|
| row | int |数据透视表目标区域左上角单元格的行索引。|
| column | int |数据透视表目标区域左上角单元格的列索引。|
| table_name | str |新数据透视表的名称。|



### 也可以看看
* 模块 [aspose.cells.pivot](../../)
* 类 [PivotTableCollection](/cells/zh/python-net/aspose.cells.pivot/pivottablecollection)
