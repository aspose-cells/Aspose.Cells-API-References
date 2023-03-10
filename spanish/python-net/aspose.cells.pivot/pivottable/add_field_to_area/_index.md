---
title: add_field_to_area método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 30
url: /es/python-net/aspose.cells.pivot/pivottable/add_field_to_area/
is_root: false
---
##  add_field_to_area(field_type, field_name) {#PivotFieldType-str}
Agrega el campo al área específica.


###  Devoluciones

La posición del campo en los campos específicos. Si no hay ningún campo con ese nombre, devuelva -1.


```python
def add_field_to_area(self, field_type, field_name):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| field_type | [PivotFieldType](/cells/es/python-net/aspose.cells.pivot/pivotfieldtype) | El tipo de área de campos.|
| field_name | str | El nombre en los campos base.|


##  add_field_to_area(field_type, base_field_index) {#PivotFieldType-int}
Agrega el campo al área específica.


###  Devoluciones

La posición del campo en los campos específicos.


```python
def add_field_to_area(self, field_type, base_field_index):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| field_type | [PivotFieldType](/cells/es/python-net/aspose.cells.pivot/pivotfieldtype) | El tipo de área de campos.|
| base_field_index | int | El índice de campo en los campos base.|


##  add_field_to_area(field_type, pivot_field) {#PivotFieldType-PivotField}
Agrega el campo al área específica.


###  Devoluciones

la posición del campo en los campos específicos.


```python
def add_field_to_area(self, field_type, pivot_field):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| field_type | [PivotFieldType](/cells/es/python-net/aspose.cells.pivot/pivotfieldtype) | el tipo de área de campos.|
| pivot_field | [PivotField](/cells/es/python-net/aspose.cells.pivot/pivotfield) | el campo en los campos base.|



###  Ver también
* módulo [aspose.cells.pivot](../../)
* clase [PivotTable](/cells/es/python-net/aspose.cells.pivot/pivottable)
