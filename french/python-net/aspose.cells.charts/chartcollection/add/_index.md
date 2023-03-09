---
title: add méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 20
url: /fr/python-net/aspose.cells.charts/chartcollection/add/
is_root: false
---
##  add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column) {#ChartType-int-int-int-int}
Ajoute un graphique à la collection.


###  Retour

[Chart](/cells/fr/python-net/aspose.cells.charts/chart) indice d'objet.


```python
def add(self, type, upper_left_row, upper_left_column, lower_right_row, lower_right_column):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| type | [ChartType](/cells/fr/python-net/aspose.cells.charts/charttype) | Type de graphique|
| upper_left_row | int | Index de ligne en haut à gauche.|
| upper_left_column | int | Index de la colonne en haut à gauche.|
| lower_right_row | int | Index de ligne en bas à droite|
| lower_right_column | int | Index de la colonne en bas à droite|


##  add(type, data_range, top_row, left_column, right_row, bottom_column) {#ChartType-str-int-int-int-int}
Ajoute un graphique à la collection.


###  Retour

[Chart](/cells/fr/python-net/aspose.cells.charts/chart) indice d'objet.


```python
def add(self, type, data_range, top_row, left_column, right_row, bottom_column):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| type | [ChartType](/cells/fr/python-net/aspose.cells.charts/charttype) | Type de graphique|
| data_range | str | Spécifie la plage de données du graphique|
| top_row | int | Index de ligne en haut à gauche.|
| left_column | int | Index de la colonne en haut à gauche.|
| right_row | int | Index de ligne en bas à droite|
| bottom_column | int | Index de la colonne en bas à droite|
###  Remarques

REMARQUE : ce membre est désormais obsolète.
veuillez utiliser la propriété [ChartCollection.add(type, upper_left_row, upper_left_column, lower_right_row, lower_right_column)](/cells/fr/python-net/aspose.cells.charts/chartcollection/add).
 Cette propriété sera supprimée 12 mois plus tard depuis mai 2022.
Aspose s'excuse pour tout inconvénient que vous pourriez avoir rencontré.

##  add(data, data_range, is_vertical, top_row, left_column, right_row, bottom_column) {#bytes-str-bool-int-int-int-int}
Ajoute un graphique avec un modèle prédéfini.


###  Retour

[Chart](/cells/fr/python-net/aspose.cells.charts/chart) indice d'objet.


```python
def add(self, data, data_range, is_vertical, top_row, left_column, right_row, bottom_column):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| data | bytes | Les données du fichier de modèle de graphique (.crtx).|
| data_range | str | Spécifie la plage de données du graphique|
| is_vertical | bool | Spécifie s'il faut tracer la série à partir d'une plage de valeurs de cellule par ligne ou par colonne.|
| top_row | int | Index de ligne en haut à gauche.|
| left_column | int | Index de la colonne en haut à gauche.|
| right_row | int | Index de ligne en bas à droite|
| bottom_column | int | Index de la colonne en bas à droite|


##  add(type, data_range, is_vertical, top_row, left_column, right_row, bottom_column) {#ChartType-str-bool-int-int-int-int}
Ajoute un graphique à la collection.


###  Retour

[Chart](/cells/fr/python-net/aspose.cells.charts/chart) indice d'objet.


```python
def add(self, type, data_range, is_vertical, top_row, left_column, right_row, bottom_column):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| type | [ChartType](/cells/fr/python-net/aspose.cells.charts/charttype) | Type de graphique|
| data_range | str | Spécifie la plage de données du graphique|
| is_vertical | bool | Spécifie s'il faut tracer la série à partir d'une plage de valeurs de cellule par ligne ou par colonne.|
| top_row | int | Index de ligne en haut à gauche.|
| left_column | int | Index de la colonne en haut à gauche.|
| right_row | int | Index de ligne en bas à droite|
| bottom_column | int | Index de la colonne en bas à droite|



###  Voir également
* module [aspose.cells.charts](../../)
* classe [Chart](/cells/fr/python-net/aspose.cells.charts/chart)
* classe [ChartCollection](/cells/fr/python-net/aspose.cells.charts/chartcollection)
