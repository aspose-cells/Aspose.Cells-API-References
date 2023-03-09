---
title: add_label méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 130
url: /fr/python-net/aspose.cells.drawing/shapecollection/add_label/
is_root: false
---
##  add_label(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Ajoute une étiquette à la feuille de calcul.


###  Retour

Un objet étiquette.


```python
def add_label(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| upper_left_row | int | Index de ligne en haut à gauche.|
| top | int | Représente le décalage vertical de Label par rapport à sa ligne de gauche, en pixels.|
| upper_left_column | int | Index de la colonne en haut à gauche.|
| left | int | Représente le décalage horizontal de Label par rapport à sa colonne de gauche, en pixels.|
| height | int | Représente la hauteur de Label, en unité de pixel.|
| width | int | Représente la largeur de Label, en unité de pixel.|

###  Exemples

```python

# add a label
label = shapes.add_label(1, 0, 1, 0, 100, 50)

```



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/fr/python-net/aspose.cells.drawing/shapecollection)
