---
title: add yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 20
url: /tr/python-net/aspose.cells.drawing/picturecollection/add/
is_root: false
---
##  add(upper_left_row, upper_left_column, stream) {#int-int-io.RawIOBase}
Koleksiyona bir resim ekler.


###  İadeler

[Picture](/cells/tr/python-net/aspose.cells.drawing/picture) nesne dizini.


```python
def add(self, upper_left_row, upper_left_column, stream):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| upper_left_row | int | Sol üst sıra dizini.|
| upper_left_column | int | Sol üst sütun dizini.|
| stream | io.RawIOBase | Görüntü verilerini içeren akış nesnesi.|

###  Örnek

```python

# add a picture
with open("image.jpg", "rb") as fs:
    pictures.add(1, 1, fs)

```


##  add(upper_left_row, upper_left_column, file_name) {#int-int-str}
Koleksiyona bir resim ekler.


###  İadeler

[Picture](/cells/tr/python-net/aspose.cells.drawing/picture) nesne dizini.


```python
def add(self, upper_left_row, upper_left_column, file_name):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| upper_left_row | int | Sol üst sıra dizini.|
| upper_left_column | int | Sol üst sütun dizini.|
| file_name | str | Görüntü dosya adı.|

###  Örnek

```python

# add a picture
pictures.add(1, 1, "image.jpg")

```


##  add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream) {#int-int-int-int-io.RawIOBase}
Koleksiyona bir resim ekler.


###  İadeler

[Picture](/cells/tr/python-net/aspose.cells.drawing/picture) nesne dizini.


```python
def add(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream):
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
    pictures.add(1, 1, 5, 5, fs)

```


##  add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name) {#int-int-int-int-str}
Koleksiyona bir resim ekler.


###  İadeler

[Picture](/cells/tr/python-net/aspose.cells.drawing/picture) nesne dizini.


```python
def add(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| upper_left_row | int | Sol üst sıra dizini.|
| upper_left_column | int | Sol üst sütun dizini.|
| lower_right_row | int | Sağ alt sıra dizini|
| lower_right_column | int | Sağ alt sütun dizini|
| file_name | str | Görüntü dosya adı.|

###  Örnek

```python

# add a picture
pictures.add(1, 1, 5, 5, "image.jpg")

```


##  add(upper_left_row, upper_left_column, stream, width_scale, height_scale) {#int-int-io.RawIOBase-int-int}
Koleksiyona bir resim ekler.


###  İadeler

[Picture](/cells/tr/python-net/aspose.cells.drawing/picture) nesne dizini.


```python
def add(self, upper_left_row, upper_left_column, stream, width_scale, height_scale):
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
    pictures.add(1, 1, fs, 50, 50)

```


##  add(upper_left_row, upper_left_column, file_name, width_scale, height_scale) {#int-int-str-int-int}
Koleksiyona bir resim ekler.


###  İadeler

[Picture](/cells/tr/python-net/aspose.cells.drawing/picture) nesne dizini.


```python
def add(self, upper_left_row, upper_left_column, file_name, width_scale, height_scale):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| upper_left_row | int | Sol üst sıra dizini.|
| upper_left_column | int | Sol üst sütun dizini.|
| file_name | str | Görüntü dosya adı.|
| width_scale | int | Görüntü genişliği ölçeği, yüzde.|
| height_scale | int | Görüntü yüksekliği ölçeği, yüzde.|

###  Örnek

```python

# add a picture
pictures.add(1, 1, "image.jpg", 50, 50)

```



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [Picture](/cells/tr/python-net/aspose.cells.drawing/picture)
* sınıf [PictureCollection](/cells/tr/python-net/aspose.cells.drawing/picturecollection)
