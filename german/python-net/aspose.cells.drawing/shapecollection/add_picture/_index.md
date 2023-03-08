---
title: add_picture Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 210
url: /de/python-net/aspose.cells.drawing/shapecollection/add_picture/
is_root: false
---
##  add_picture(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream) {#int-int-int-int-io.RawIOBase}
Fügt der Sammlung ein Bild hinzu.


###  Kehrt zurück

[Picture](/cells/de/python-net/aspose.cells.drawing/picture) Bildobjekt.


```python
def add_picture(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| upper_left_row | int | Zeilenindex oben links.|
| upper_left_column | int |Spaltenindex oben links.|
| lower_right_row | int | Zeilenindex unten rechts|
| lower_right_column | int | Spaltenindex unten rechts|
| stream | io.RawIOBase | Stream-Objekt, das die Bilddaten enthält.|

###  Beispiel

```python

# add a picture
with open("image.jpg", "rb") as fs:
    picture = shapes.add_picture(1, 0, 1, 0, fs)

```


##  add_picture(upper_left_row, upper_left_column, stream, width_scale, height_scale) {#int-int-io.RawIOBase-int-int}
Fügt der Sammlung ein Bild hinzu.


###  Kehrt zurück

[Picture](/cells/de/python-net/aspose.cells.drawing/picture) Bildobjekt.


```python
def add_picture(self, upper_left_row, upper_left_column, stream, width_scale, height_scale):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| upper_left_row | int | Zeilenindex oben links.|
| upper_left_column | int |Spaltenindex oben links.|
| stream | io.RawIOBase | Stream-Objekt, das die Bilddaten enthält.|
| width_scale | int | Maßstab der Bildbreite, ein Prozentsatz.|
| height_scale | int | Maßstab der Bildhöhe, ein Prozentsatz.|

###  Beispiel

```python

# add a picture
with open("image.jpg", "rb") as fs:
    picture = shapes.add_picture(1, 1, fs, 50, 60)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [Picture](/cells/de/python-net/aspose.cells.drawing/picture)
* Klasse [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection)
