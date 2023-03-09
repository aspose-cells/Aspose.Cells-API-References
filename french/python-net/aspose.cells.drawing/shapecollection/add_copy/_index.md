---
title: add_copy méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 90
url: /fr/python-net/aspose.cells.drawing/shapecollection/add_copy/
is_root: false
---
##  add_copy(source_shape, upper_left_row, top, upper_left_column, left) {#Shape-int-int-int-int}
Ajoute et copie une forme dans la feuille de calcul.


###  Retour

Le nouvel index d'objet de forme.


```python
def add_copy(self, source_shape, upper_left_row, top, upper_left_column, left):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| source_shape | [Shape](/cells/fr/python-net/aspose.cells.drawing/shape) | Forme source.|
| upper_left_row | int | Index de ligne en haut à gauche.|
| top | int |Représente le décalage vertical de la case à cocher par rapport à sa ligne de gauche, en unité de pixel.|
| upper_left_column | int | Index de la colonne en haut à gauche.|
| left | int | Représente le décalage horizontal de la zone de texte par rapport à sa colonne de gauche, en unité de pixel.|

###  Exemples

```python

# add a shape
rectangle = shapes.add_rectangle(2, 0, 2, 0, 130, 130)
# copy
shapes.add_copy(rectangle, 7, 0, 7, 0)

```



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/fr/python-net/aspose.cells.drawing/shapecollection)
