---
title: group Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 420
url: /de/python-net/aspose.cells.drawing/shapecollection/group/
is_root: false
---
##  group(group_items) {#list}
Gruppieren Sie die Formen.


###  Kehrt zurück

Geben Sie die Form group zurück.


```python
def group(self, group_items):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| group_items | list | die Gruppenartikel.|
###  Bemerkungen

Die Form in den groupItems sollte nicht gruppiert werden.
Die Form muss sich in dieser Shapes-Sammlung befinden.
###  Beispiele

```python

# add first shape
shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
shapes.add_rectangle(6, 0, 2, 0, 30, 30)
shapesArr = [shapes[0], shapes[1]]
groupShape = shapes.group(shapesArr)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection)
