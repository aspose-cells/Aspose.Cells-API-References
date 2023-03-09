---
title: add_list_box méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 170
url: /fr/python-net/aspose.cells.drawing/shapecollection/add_list_box/
is_root: false
---
##  add_list_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Ajoute un ListBox à la feuille de calcul.


###  Retour

Un objet ListBox.


```python
def add_list_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| upper_left_row | int | Index de ligne en haut à gauche.|
| top | int | Représente le décalage vertical de ListBox par rapport à sa ligne de gauche, en unité de pixel.|
| upper_left_column | int | Index de la colonne en haut à gauche.|
| left | int | Représente le décalage horizontal de ListBox par rapport à sa colonne de gauche, en unité de pixel.|
| height | int | Représente la hauteur de ListBox, en unité de pixel.|
| width | int | Représente la largeur de ListBox, en unité de pixel.|

###  Exemples

```python

# add a list box
listBox = shapes.add_list_box(1, 0, 1, 0, 100, 50)

```



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/fr/python-net/aspose.cells.drawing/shapecollection)
