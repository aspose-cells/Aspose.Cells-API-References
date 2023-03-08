---
title: add_field_to_area方法
second_title: Aspose.Cells for Python via .NET API 参考资料
description:
type: docs
weight: 30
url: /zh/python-net/aspose.cells.pivot/pivottable/add_field_to_area/
is_root: false
---
##  add_field_to_area(field_type, field_name) {#PivotFieldType-str}
将字段添加到特定区域。


### 返回

特定字段中的字段位置。如果没有以它命名的字段，则返回-1。


```python
def add_field_to_area(self, field_type, field_name):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| field_type | [PivotFieldType](/cells/zh/python-net/aspose.cells.pivot/pivotfieldtype) |字段区域类型。|
| field_name | str |基本字段中的名称。|


##  add_field_to_area(field_type, base_field_index) {#PivotFieldType-int}
将字段添加到特定区域。


### 返回

特定字段中的字段位置。


```python
def add_field_to_area(self, field_type, base_field_index):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| field_type | [PivotFieldType](/cells/zh/python-net/aspose.cells.pivot/pivotfieldtype) |字段区域类型。|
| base_field_index | int |基字段中的字段索引。|


##  add_field_to_area(field_type, pivot_field) {#PivotFieldType-PivotField}
将字段添加到特定区域。


### 返回

特定字段中的字段位置。


```python
def add_field_to_area(self, field_type, pivot_field):
    ...
```


|范围|类型|描述|
| :- | :- | :- |
| field_type | [PivotFieldType](/cells/zh/python-net/aspose.cells.pivot/pivotfieldtype) |字段区域类型。|
| pivot_field | [PivotField](/cells/zh/python-net/aspose.cells.pivot/pivotfield) |基域中的域。|



### 也可以看看
* 模块 [aspose.cells.pivot](../../)
* 类 [PivotTable](/cells/zh/python-net/aspose.cells.pivot/pivottable)
