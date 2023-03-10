---
title: group yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 420
url: /tr/python-net/aspose.cells.drawing/shapecollection/group/
is_root: false
---
##  group(group_items) {#list}
Şekilleri gruplandırın.


###  İadeler

group şeklini döndürün.


```python
def group(self, group_items):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| group_items | list | grup öğeleri.|
###  Notlar

groupItems içindeki şekil gruplandırılmamalıdır.
Şekil, bu Şekiller koleksiyonunda olmalıdır.
###  Örnek

```python

# add first shape
shapes.add_rectangle(2, 0, 2, 0, 50, 50)
# add second shape
shapes.add_rectangle(6, 0, 2, 0, 30, 30)
shapesArr = [shapes[0], shapes[1]]
groupShape = shapes.group(shapesArr)

```



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [ShapeCollection](/cells/tr/python-net/aspose.cells.drawing/shapecollection)
