---
title: add_shape méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 260
url: /fr/python-net/aspose.cells.drawing/shapecollection/add_shape/
is_root: false
---
##  add_shape(type, upper_left_row, top, upper_left_column, left, height, width) {#MsoDrawingType-int-int-int-int-int-int}
Ajoute une forme à la feuille de calcul.


###  Retour

Un objet Shape.


```python
def add_shape(self, type, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| type | [MsoDrawingType](/cells/fr/python-net/aspose.cells.drawing/msodrawingtype) | Type de dessin Mso.|
| upper_left_row | int | Index de ligne en haut à gauche.|
| top | int | Représente le décalage vertical de Shape par rapport à sa ligne de gauche, en pixels.|
| upper_left_column | int | Index de la colonne en haut à gauche.|
| left | int | Représente le décalage horizontal de Shape par rapport à sa colonne de gauche, en pixels.|
| height | int | Représente la hauteur de Shape, en unité de pixel.|
| width | int | Représente la largeur de Shape, en unité de pixel.|
###  Remarques

Le type ne peut pas être Chart/Comment/Picture/OleObject/Polygon/DialogBox
###  Exemple


```python
from aspose.cells.drawing import MsoDrawingType

# Add a shape of the specified type
shapeByType = shapes.add_shape(MsoDrawingType.CELLS_DRAWING, 1, 0, 1, 0, 100, 50)

```



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/fr/python-net/aspose.cells.drawing/shapecollection)
