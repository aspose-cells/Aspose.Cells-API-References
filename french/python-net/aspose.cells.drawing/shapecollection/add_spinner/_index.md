---
title: add_spinner méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 290
url: /fr/python-net/aspose.cells.drawing/shapecollection/add_spinner/
is_root: false
---
##  add_spinner(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Ajoute un Spinner à la feuille de calcul.


###  Retour

Un objet Spinner.


```python
def add_spinner(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| upper_left_row | int | Index de ligne en haut à gauche.|
| top | int |Représente le décalage vertical de Spinner par rapport à sa ligne de gauche, en unité de pixel.|
| upper_left_column | int | Index de la colonne en haut à gauche.|
| left | int | Représente le décalage horizontal de Spinner par rapport à sa colonne de gauche, en unité de pixel.|
| height | int | Représente la hauteur de Spinner, en unité de pixel.|
| width | int | Représente la largeur de Spinner, en unité de pixel.|

###  Exemple

```python

# add a spinner
spinner = shapes.add_spinner(1, 0, 1, 0, 100, 50)

```



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/fr/python-net/aspose.cells.drawing/shapecollection)
