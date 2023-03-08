---
title: ungroup Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 450
url: /de/python-net/aspose.cells.drawing/shapecollection/ungroup/
is_root: false
---
##  ungroup(group) {#GroupShape}
Hebt die Gruppierung der Formelemente auf.



```python
def ungroup(self, group):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| group | [GroupShape](/cells/de/python-net/aspose.cells.drawing/groupshape) | Die Gruppenform.|
###  Bemerkungen

Wenn das Gruppen-Shape von einem anderen Gruppen-Shape gruppiert wird, wird nichts getan.
###  Beispiel


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



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection)
