---
title: add_rectangle méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 240
url: /fr/python-net/aspose.cells.drawing/shapecollection/add_rectangle/
is_root: false
---
##  add_rectangle(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Ajoute un RectangleShape à la feuille de calcul.


###  Retour

Un objet RectangleShape.


```python
def add_rectangle(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| upper_left_row | int | Index de ligne en haut à gauche.|
| top | int | Représente le décalage vertical de RectangleShape par rapport à sa ligne de gauche, en unité de pixel.|
| upper_left_column | int | Index de la colonne en haut à gauche.|
| left | int | Représente le décalage horizontal de RectangleShape par rapport à sa colonne de gauche, en pixels.|
| height | int | Représente la hauteur de RectangleShape, en unité de pixel.|
| width | int | Représente la largeur de RectangleShape, en unité de pixel.|

###  Exemples

```python

#  add a rectangle
rectangleShape = shapes.add_rectangle(2, 0, 2, 0, 130, 130)

```



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/fr/python-net/aspose.cells.drawing/shapecollection)
