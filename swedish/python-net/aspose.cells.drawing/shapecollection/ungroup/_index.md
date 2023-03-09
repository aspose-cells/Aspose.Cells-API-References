---
title: ungroup metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 450
url: /sv/python-net/aspose.cells.drawing/shapecollection/ungroup/
is_root: false
---
##  ungroup(group) {#GroupShape}
Dela upp formobjekten.



```python
def ungroup(self, group):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| group | [GroupShape](/cells/sv/python-net/aspose.cells.drawing/groupshape) | Gruppformen.|
###  Anmärkningar

Om gruppformen grupperas efter en annan gruppform kommer ingenting att göras.
###  Exempel


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



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection)
