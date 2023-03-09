---
title: group metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 420
url: /sv/python-net/aspose.cells.drawing/shapecollection/group/
is_root: false
---
##  group(group_items) {#list}
Gruppera formerna.


###  Returnerar

Lämna tillbaka formen group.


```python
def group(self, group_items):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| group_items | list | gruppobjekten.|
###  Anmärkningar

Formen i groupItems ska inte grupperas.
Formen måste finnas i den här Shapes-kollektionen.
###  Exempel

```python

# add first shape
shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
shapes.add_rectangle(6, 0, 2, 0, 30, 30)
shapesArr = [shapes[0], shapes[1]]
groupShape = shapes.group(shapesArr)

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection)
