---
title: add_field_to_area method
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 30
url: /python-net/aspose.cells.pivot/pivottable/add_field_to_area/
is_root: false
---

## add_field_to_area(field_type, field_name) {#PivotFieldType-str}

Adds the field to the specific area.

### Returns 


The field position in the specific fields.If there is no field named as it, return -1.


```python
def add_field_to_area(self, field_type, field_name):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| field_type | [PivotFieldType](/cells/python-net/aspose.cells.pivot/pivotfieldtype) | The fields area type. |
| field_name | str | The name in the base fields. |


## add_field_to_area(field_type, base_field_index) {#PivotFieldType-int}

Adds the field to the specific area.

### Returns 


The field position in the specific fields.


```python
def add_field_to_area(self, field_type, base_field_index):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| field_type | [PivotFieldType](/cells/python-net/aspose.cells.pivot/pivotfieldtype) | The fields area type. |
| base_field_index | int | The field index in the base fields. |


## add_field_to_area(field_type, pivot_field) {#PivotFieldType-PivotField}

Adds the field to the specific area.

### Returns 


the field position in the specific fields.


```python
def add_field_to_area(self, field_type, pivot_field):
    ...
```


| Parameter | Type | Description |
| :- | :- | :- |
| field_type | [PivotFieldType](/cells/python-net/aspose.cells.pivot/pivotfieldtype) | the fields area type. |
| pivot_field | [PivotField](/cells/python-net/aspose.cells.pivot/pivotfield) | the field in the base fields. |



### See Also
* module [aspose.cells.pivot](../../)
* class [PivotTable](/cells/python-net/aspose.cells.pivot/pivottable)
