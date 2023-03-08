---
title: delete_shape Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 410
url: /de/python-net/aspose.cells.drawing/shapecollection/delete_shape/
is_root: false
---
##  delete_shape(shape) {#Shape}
Löschen Sie eine Form. Wenn sich die Form in der Gruppe befindet oder eine Kommentarform ist, wird sie nicht gelöscht.



```python
def delete_shape(self, shape):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| shape | [Shape](/cells/de/python-net/aspose.cells.drawing/shape) |  |

###  Beispiel

```python

# add first shape
firstShape = shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
secondShape = shapes.add_rectangle(6, 0, 2, 0, 30, 30)
# del
shapes.delete_shape(firstShape)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection)
