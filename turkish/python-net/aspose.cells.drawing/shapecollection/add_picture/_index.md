---
title: add_picture yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 210
url: /tr/python-net/aspose.cells.drawing/shapecollection/add_picture/
is_root: false
---
##  add_picture(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream) {#int-int-int-int-io.RawIOBase}
Koleksiyona bir resim ekler.


###  İadeler

[Picture](/cells/tr/python-net/aspose.cells.drawing/picture) Resim nesnesi.


```python
def add_picture(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| upper_left_row | int | Sol üst sıra dizini.|
| upper_left_column | int | Sol üst sütun dizini.|
| lower_right_row | int | Sağ alt sıra dizini|
| lower_right_column | int | Sağ alt sütun dizini|
| stream | io.RawIOBase | Görüntü verilerini içeren akış nesnesi.|

###  Örnek

```python

# add a picture
with open("image.jpg", "rb") as fs:
    picture = shapes.add_picture(1, 0, 1, 0, fs)

```


##  add_picture(upper_left_row, upper_left_column, stream, width_scale, height_scale) {#int-int-io.RawIOBase-int-int}
Koleksiyona bir resim ekler.


###  İadeler

[Picture](/cells/tr/python-net/aspose.cells.drawing/picture) Resim nesnesi.


```python
def add_picture(self, upper_left_row, upper_left_column, stream, width_scale, height_scale):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| upper_left_row | int | Sol üst sıra dizini.|
| upper_left_column | int | Sol üst sütun dizini.|
| stream | io.RawIOBase | Görüntü verilerini içeren akış nesnesi.|
| width_scale | int | Görüntü genişliği ölçeği, yüzde.|
| height_scale | int | Görüntü yüksekliği ölçeği, yüzde.|

###  Örnek

```python

# add a picture
with open("image.jpg", "rb") as fs:
    picture = shapes.add_picture(1, 1, fs, 50, 60)

```



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [Picture](/cells/tr/python-net/aspose.cells.drawing/picture)
* sınıf [ShapeCollection](/cells/tr/python-net/aspose.cells.drawing/shapecollection)
