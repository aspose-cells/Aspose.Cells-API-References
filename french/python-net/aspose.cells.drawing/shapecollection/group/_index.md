---
title: group méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 420
url: /fr/python-net/aspose.cells.drawing/shapecollection/group/
is_root: false
---
##  group(group_items) {#list}
Regroupez les formes.


###  Retour

Renvoyez la forme group.


```python
def group(self, group_items):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| group_items | list | les éléments du groupe.|
###  Remarques

La forme dans groupItems ne doit pas être groupée.
La forme doit se trouver dans cette collection Shapes.
###  Exemple

```python

# add first shape
shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
shapes.add_rectangle(6, 0, 2, 0, 30, 30)
shapesArr = [shapes[0], shapes[1]]
groupShape = shapes.group(shapesArr)

```



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/fr/python-net/aspose.cells.drawing/shapecollection)
