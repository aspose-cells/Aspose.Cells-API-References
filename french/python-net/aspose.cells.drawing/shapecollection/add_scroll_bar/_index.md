---
title: add_scroll_bar méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 250
url: /fr/python-net/aspose.cells.drawing/shapecollection/add_scroll_bar/
is_root: false
---
##  add_scroll_bar(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Ajoute un ScrollBar à la feuille de calcul.


###  Retour

Un objet ScrollBar.


```python
def add_scroll_bar(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| upper_left_row | int | Index de ligne en haut à gauche.|
| top | int | Représente le décalage vertical de ScrollBar à partir de sa ligne de gauche, en unité de pixel.|
| upper_left_column | int | Index de la colonne en haut à gauche.|
| left | int | Représente le décalage horizontal de ScrollBar par rapport à sa colonne de gauche, en unité de pixel.|
| height | int | Représente la hauteur de ScrollBar, en unité de pixel.|
| width | int | Représente la largeur de ScrollBar, en unité de pixel.|

###  Exemple

```python

# add a scroll bar
scrollBar = shapes.add_scroll_bar(1, 0, 1, 0, 100, 50)

```



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/fr/python-net/aspose.cells.drawing/shapecollection)
