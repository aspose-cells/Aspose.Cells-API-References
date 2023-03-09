---
title: add_field_to_area méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 30
url: /fr/python-net/aspose.cells.pivot/pivottable/add_field_to_area/
is_root: false
---
##  add_field_to_area(field_type, field_name) {#PivotFieldType-str}
Ajoute le champ à la zone spécifique.


###  Retour

La position du champ dans les champs spécifiques. S'il n'y a pas de champ nommé comme celui-ci, renvoie -1.


```python
def add_field_to_area(self, field_type, field_name):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| field_type | [PivotFieldType](/cells/fr/python-net/aspose.cells.pivot/pivotfieldtype) | Le type de zone des champs.|
| field_name | str | Le nom dans les champs de base.|


##  add_field_to_area(field_type, base_field_index) {#PivotFieldType-int}
Ajoute le champ à la zone spécifique.


###  Retour

La position du champ dans les champs spécifiques.


```python
def add_field_to_area(self, field_type, base_field_index):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| field_type | [PivotFieldType](/cells/fr/python-net/aspose.cells.pivot/pivotfieldtype) | Le type de zone des champs.|
| base_field_index | int | L'index de champ dans les champs de base.|


##  add_field_to_area(field_type, pivot_field) {#PivotFieldType-PivotField}
Ajoute le champ à la zone spécifique.


###  Retour

la position du champ dans les champs spécifiques.


```python
def add_field_to_area(self, field_type, pivot_field):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| field_type | [PivotFieldType](/cells/fr/python-net/aspose.cells.pivot/pivotfieldtype) | le type de zone des champs.|
| pivot_field | [PivotField](/cells/fr/python-net/aspose.cells.pivot/pivotfield) | le champ dans les champs de base.|



###  Voir également
* module [aspose.cells.pivot](../../)
* classe [PivotTable](/cells/fr/python-net/aspose.cells.pivot/pivottable)
