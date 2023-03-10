---
title: delete_shape yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 410
url: /tr/python-net/aspose.cells.drawing/shapecollection/delete_shape/
is_root: false
---
##  delete_shape(shape) {#Shape}
Bir şekli silin. Şekil grup içindeyse veya bir yorum şekliyse silinmez.



```python
def delete_shape(self, shape):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| shape | [Shape](/cells/tr/python-net/aspose.cells.drawing/shape) |  |

###  Örnek

```python

# add first shape
firstShape = shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
secondShape = shapes.add_rectangle(6, 0, 2, 0, 30, 30)
# del
shapes.delete_shape(firstShape)

```



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [ShapeCollection](/cells/tr/python-net/aspose.cells.drawing/shapecollection)
