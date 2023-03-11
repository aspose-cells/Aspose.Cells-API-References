---
title: add_group_box méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 110
url: /fr/python-net/aspose.cells.drawing/shapecollection/add_group_box/
is_root: false
---
##  add_group_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Ajoute un GroupBox à la feuille de calcul.


###  Retour

Un objet GroupBox.


```python
def add_group_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| upper_left_row | int | Index de ligne en haut à gauche.|
| top | int | Représente le décalage vertical de GroupBox par rapport à sa ligne de gauche, en unité de pixel.|
| upper_left_column | int | Index de la colonne en haut à gauche.|
| left | int | Représente le décalage horizontal de GroupBox par rapport à sa colonne de gauche, en unité de pixel.|
| height | int | Représente la hauteur de GroupBox, en unité de pixel.|
| width | int | Représente la largeur de GroupBox, en unité de pixel.|

###  Exemple

```python

# add a group box
groupBox = shapes.add_group_box(1, 0, 1, 0, 100, 50)

```



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/fr/python-net/aspose.cells.drawing/shapecollection)
