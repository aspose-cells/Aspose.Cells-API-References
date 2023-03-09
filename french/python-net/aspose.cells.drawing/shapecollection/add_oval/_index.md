---
title: add_oval méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 200
url: /fr/python-net/aspose.cells.drawing/shapecollection/add_oval/
is_root: false
---
##  add_oval(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Ajoute un ovale à la feuille de calcul.


###  Retour

Un objet ovale.


```python
def add_oval(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| upper_left_row | int | Index de ligne en haut à gauche.|
| top | int | Représente le décalage vertical d'Oval par rapport à sa ligne de gauche, en unité de pixel.|
| upper_left_column | int |Index de la colonne en haut à gauche.|
| left | int | Représente le décalage horizontal d'Oval par rapport à sa colonne de gauche, en pixels.|
| height | int | Représente la hauteur d'Oval, en unité de pixel.|
| width | int | Représente la largeur d'Oval, en unité de pixel.|

###  Exemple

```python

# add a oval
oval = shapes.add_oval(1, 0, 1, 0, 50, 50)

```



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/fr/python-net/aspose.cells.drawing/shapecollection)
