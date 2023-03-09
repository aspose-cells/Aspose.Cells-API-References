---
title: create_range méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 190
url: /fr/python-net/aspose.cells/cells/create_range/
is_root: false
---
##  create_range(address) {#str}
Crée un objet [Range](/cells/fr/python-net/aspose.cells/range) à partir d'une adresse de la plage.


###  Retour

Un objet [Range](/cells/fr/python-net/aspose.cells/range)


```python
def create_range(self, address):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| address | str | L'adresse de la plage.|


##  create_range(upper_left_cell, lower_right_cell) {#str-str}
Crée un objet [Range](/cells/fr/python-net/aspose.cells/range) à partir d'une plage de cellules.


###  Retour

Un objet [Range](/cells/fr/python-net/aspose.cells/range)


```python
def create_range(self, upper_left_cell, lower_right_cell):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| upper_left_cell | str | Nom de cellule en haut à gauche.|
| lower_right_cell | str | Nom de cellule en bas à droite.|


##  create_range(first_index, number, is_vertical) {#int-int-bool}
Crée un objet [Range](/cells/fr/python-net/aspose.cells/range) à partir de rangées de cellules ou de colonnes de cellules.


###  Retour

Un objet [Range](/cells/fr/python-net/aspose.cells/range).


```python
def create_range(self, first_index, number, is_vertical):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| first_index | int | Index de première ligne ou index de première colonne, basé sur zéro.|
| number | int | Nombre total de lignes ou de colonnes, basées sur une.|
| is_vertical | bool | True - Plage créée à partir de colonnes de cellules. False - Plage créée à partir de rangées de cellules.|


##  create_range(first_row, first_column, total_rows, total_columns) {#int-int-int-int}
Crée un objet [Range](/cells/fr/python-net/aspose.cells/range) à partir d'une plage de cellules.


###  Retour

Un objet [Range](/cells/fr/python-net/aspose.cells/range)


```python
def create_range(self, first_row, first_column, total_rows, total_columns):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| first_row | int | Première ligne de cette gamme|
| first_column | int | Première colonne de cette plage|
| total_rows | int | Nombre de rangées|
| total_columns | int | Le nombre de colonnes|



###  Voir également
* module [aspose.cells](../../)
* classe [Cells](/cells/fr/python-net/aspose.cells/cells)
* classe [Range](/cells/fr/python-net/aspose.cells/range)
