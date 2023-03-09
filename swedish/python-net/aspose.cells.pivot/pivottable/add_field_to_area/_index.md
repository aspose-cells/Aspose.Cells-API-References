---
title: add_field_to_area metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 30
url: /sv/python-net/aspose.cells.pivot/pivottable/add_field_to_area/
is_root: false
---
##  add_field_to_area(field_type, field_name) {#PivotFieldType-str}
Lägger till fältet till det specifika området.


###  Returnerar

Fältpositionen i de specifika fälten. Om det inte finns något fält som heter det, returnera -1.


```python
def add_field_to_area(self, field_type, field_name):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| field_type | [PivotFieldType](/cells/sv/python-net/aspose.cells.pivot/pivotfieldtype) | Fältets områdestyp.|
| field_name | str |Namnet i basfälten.|


##  add_field_to_area(field_type, base_field_index) {#PivotFieldType-int}
Lägger till fältet till det specifika området.


###  Returnerar

Fältpositionen i de specifika fälten.


```python
def add_field_to_area(self, field_type, base_field_index):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| field_type | [PivotFieldType](/cells/sv/python-net/aspose.cells.pivot/pivotfieldtype) | Fältets områdestyp.|
| base_field_index | int | Fältindex i basfälten.|


##  add_field_to_area(field_type, pivot_field) {#PivotFieldType-PivotField}
Lägger till fältet till det specifika området.


###  Returnerar

fältpositionen i de specifika fälten.


```python
def add_field_to_area(self, field_type, pivot_field):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| field_type | [PivotFieldType](/cells/sv/python-net/aspose.cells.pivot/pivotfieldtype) | fältets områdestyp.|
| pivot_field | [PivotField](/cells/sv/python-net/aspose.cells.pivot/pivotfield) | fältet i basfälten.|



###  Se även
* modul [aspose.cells.pivot](../../)
* klass [PivotTable](/cells/sv/python-net/aspose.cells.pivot/pivottable)
