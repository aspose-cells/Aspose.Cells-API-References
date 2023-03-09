---
title: ungroup méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 450
url: /fr/python-net/aspose.cells.drawing/shapecollection/ungroup/
is_root: false
---
##  ungroup(group) {#GroupShape}
Dissociez les éléments de forme.



```python
def ungroup(self, group):
    ...
```


| Paramètres| Taper| Description|
| :- | :- | :- |
| group | [GroupShape](/cells/fr/python-net/aspose.cells.drawing/groupshape) | La forme du groupe.|
###  Remarques

Si la forme de groupe est groupée par une autre forme de groupe, rien ne sera fait.
###  Exemples


```python

# add first shape
shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
shapes.add_rectangle(6, 0, 2, 0, 30, 30)
# group
shapesArr = [shapes[0], shapes[1]]
groupShape = shapes.group(shapesArr)
# ungroup
shapes.ungroup(groupShape)

```



###  Voir également
* module [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/fr/python-net/aspose.cells.drawing/shapecollection)
