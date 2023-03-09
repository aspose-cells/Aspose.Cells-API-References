---
title: delete_shape metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 410
url: /sv/python-net/aspose.cells.drawing/shapecollection/delete_shape/
is_root: false
---
##  delete_shape(shape) {#Shape}
Ta bort en form. Om formen finns i gruppen eller är en kommentarsform kommer den inte att tas bort.



```python
def delete_shape(self, shape):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| shape | [Shape](/cells/sv/python-net/aspose.cells.drawing/shape) |  |

###  Exempel

```python

# add first shape
firstShape = shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
secondShape = shapes.add_rectangle(6, 0, 2, 0, 30, 30)
# del
shapes.delete_shape(firstShape)

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection)
