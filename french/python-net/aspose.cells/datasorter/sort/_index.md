---
title: sort méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 40
url: /fr/python-net/aspose.cells/datasorter/sort/
is_root: false
---
##  sort() {#}
Triez les données dans la plage.


###  Retour

les indices d'origine (position absolue, par exemple, la colonne A est 0, B est 1, ...) des lignes/colonnes triées.
Si aucune ligne/colonne ne doit être déplacée par cette opération de tri, null sera renvoyé.


```python
def sort(self):
    ...
```




##  sort(cells, area) {#Cells-CellArea}
Trier les données de la zone.


###  Retour

les indices d'origine (position absolue, par exemple, la colonne A est 0, B est 1, ...) des lignes/colonnes triées.
Si aucune ligne/colonne ne doit être déplacée par cette opération de tri, null sera renvoyé.


```python
def sort(self, cells, area):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| cells | [Cells](/cells/fr/python-net/aspose.cells/cells) | Les cellules contiennent la zone de données.|
| area | [CellArea](/cells/fr/python-net/aspose.cells/cellarea) | La surface nécessaire pour trier|


##  sort(cells, start_row, start_column, end_row, end_column) {#Cells-int-int-int-int}
Trie les données de la zone.


###  Retour

les indices d'origine (position absolue, par exemple, la colonne A est 0, B est 1, ...) des lignes/colonnes triées.
Si aucune ligne/colonne ne doit être déplacée par cette opération de tri, null sera renvoyé.


```python
def sort(self, cells, start_row, start_column, end_row, end_column):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| cells | [Cells](/cells/fr/python-net/aspose.cells/cells) | Les cellules contiennent la zone de données.|
| start_row | int | La ligne de départ de la zone.|
| start_column | int | La colonne de départ de la zone.|
| end_row | int | La rangée de fin de la zone.|
| end_column | int | La colonne de fin de la zone.|



###  Voir également
* module [aspose.cells](../../)
* classe [DataSorter](/cells/fr/python-net/aspose.cells/datasorter)
