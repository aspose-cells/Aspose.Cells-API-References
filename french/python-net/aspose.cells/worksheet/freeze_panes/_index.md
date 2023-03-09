---
title: freeze_panes méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 120
url: /fr/python-net/aspose.cells/worksheet/freeze_panes/
is_root: false
---
##  freeze_panes(cell_name, freezed_rows, freezed_columns) {#str-int-int}
Gèle les volets au niveau de la cellule spécifiée dans la feuille de calcul.



```python
def freeze_panes(self, cell_name, freezed_rows, freezed_columns):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| cell_name | str | Cell nom.|
| freezed_rows | int | Nombre de lignes visibles dans le volet supérieur, pas plus que l'index de ligne.|
| freezed_columns | int | Nombre de colonnes visibles dans le volet de gauche, pas plus que l'index de colonne.|
###  Remarques

L'index de ligne et l'index de colonne ne peuvent pas tous être nuls.
ne peuvent pas non plus tous être nuls.

##  freeze_panes(row, column, freezed_rows, freezed_columns) {#int-int-int-int}
Gèle les volets au niveau de la cellule spécifiée dans la feuille de calcul.



```python
def freeze_panes(self, row, column, freezed_rows, freezed_columns):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| row | int | Indice de ligne.|
| column | int | Indice de colonne.|
| freezed_rows | int | Nombre de lignes visibles dans le volet supérieur, pas plus que l'index de ligne.|
| freezed_columns | int | Nombre de colonnes visibles dans le volet de gauche, pas plus que l'index de colonne.|
###  Remarques

L'index de ligne et l'index de colonne ne peuvent pas tous être nuls.
ne peuvent pas non plus tous être nuls.


Les deux premiers paramètres spécifient la position gelée et les deux derniers paramètres spécifient la zone gelée sur le volet supérieur gauche.


###  Voir également
* module [aspose.cells](../../)
* classe [Worksheet](/cells/fr/python-net/aspose.cells/worksheet)
