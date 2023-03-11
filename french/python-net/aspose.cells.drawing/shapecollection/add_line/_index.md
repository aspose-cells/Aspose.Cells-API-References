---
title: add_line méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 150
url: /fr/python-net/aspose.cells.drawing/shapecollection/add_line/
is_root: false
---
##  add_line(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Ajoute un LineShape à la feuille de calcul.


###  Retour

Un objet LineShape.


```python
def add_line(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| upper_left_row | int | Index de ligne en haut à gauche.|
| top | int | Représente le décalage vertical de LineShape par rapport à sa ligne de gauche, en pixels.|
| upper_left_column | int | Index de la colonne en haut à gauche.|
| left | int | Représente le décalage horizontal de LineShape par rapport à sa colonne de gauche, en pixels.|
| height | int | Représente la hauteur de LineShape, en unité de pixel.|
| width | int | Représente la largeur de LineShape, en unité de pixel.|

###  Exemple

```python

#  add a line object
lineShape = shapes.add_line(1, 0, 1, 0, 100, 50)

```



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/fr/python-net/aspose.cells.drawing/shapecollection)
