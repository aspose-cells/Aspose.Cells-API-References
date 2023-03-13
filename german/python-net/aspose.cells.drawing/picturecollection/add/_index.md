---
title: add Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 20
url: /de/python-net/aspose.cells.drawing/picturecollection/add/
is_root: false
---
##  add(upper_left_row, upper_left_column, stream) {#int-int-io.RawIOBase}
Fügt der Sammlung ein Bild hinzu.


###  Kehrt zurück

[Picture](/cells/de/python-net/aspose.cells.drawing/picture) Objektindex.


```python
def add(self, upper_left_row, upper_left_column, stream):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| upper_left_row | int | Zeilenindex oben links.|
| upper_left_column | int | Spaltenindex oben links.|
| stream | io.RawIOBase | Stream-Objekt, das die Bilddaten enthält.|

###  Beispiel

```python

# add a picture
with open("image.jpg", "rb") as fs:
    pictures.add(1, 1, fs)

```


##  add(upper_left_row, upper_left_column, file_name) {#int-int-str}
Fügt der Sammlung ein Bild hinzu.


###  Kehrt zurück

[Picture](/cells/de/python-net/aspose.cells.drawing/picture) Objektindex.


```python
def add(self, upper_left_row, upper_left_column, file_name):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| upper_left_row | int | Zeilenindex oben links.|
| upper_left_column | int | Spaltenindex oben links.|
| file_name | str | Bilddateiname.|

###  Beispiel

```python

# add a picture
pictures.add(1, 1, "image.jpg")

```


##  add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream) {#int-int-int-int-io.RawIOBase}
Fügt der Sammlung ein Bild hinzu.


###  Kehrt zurück

[Picture](/cells/de/python-net/aspose.cells.drawing/picture) Objektindex.


```python
def add(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, stream):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| upper_left_row | int | Zeilenindex oben links.|
| upper_left_column | int | Spaltenindex oben links.|
| lower_right_row | int | Zeilenindex unten rechts|
| lower_right_column | int | Spaltenindex unten rechts|
| stream | io.RawIOBase | Stream-Objekt, das die Bilddaten enthält.|

###  Beispiel

```python

# add a picture
with open("image.jpg", "rb") as fs:
    pictures.add(1, 1, 5, 5, fs)

```


##  add(upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name) {#int-int-int-int-str}
Fügt der Sammlung ein Bild hinzu.


###  Kehrt zurück

[Picture](/cells/de/python-net/aspose.cells.drawing/picture) Objektindex.


```python
def add(self, upper_left_row, upper_left_column, lower_right_row, lower_right_column, file_name):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| upper_left_row | int | Zeilenindex oben links.|
| upper_left_column | int | Spaltenindex oben links.|
| lower_right_row | int | Zeilenindex unten rechts|
| lower_right_column | int | Spaltenindex unten rechts|
| file_name | str | Bilddateiname.|

###  Beispiel

```python

# add a picture
pictures.add(1, 1, 5, 5, "image.jpg")

```


##  add(upper_left_row, upper_left_column, stream, width_scale, height_scale) {#int-int-io.RawIOBase-int-int}
Fügt der Sammlung ein Bild hinzu.


###  Kehrt zurück

[Picture](/cells/de/python-net/aspose.cells.drawing/picture) Objektindex.


```python
def add(self, upper_left_row, upper_left_column, stream, width_scale, height_scale):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| upper_left_row | int | Zeilenindex oben links.|
| upper_left_column | int | Spaltenindex oben links.|
| stream | io.RawIOBase | Stream-Objekt, das die Bilddaten enthält.|
| width_scale | int | Maßstab der Bildbreite, ein Prozentsatz.|
| height_scale | int | Maßstab der Bildhöhe, ein Prozentsatz.|

###  Beispiel

```python

# add a picture
with open("image.jpg", "rb") as fs:
    pictures.add(1, 1, fs, 50, 50)

```


##  add(upper_left_row, upper_left_column, file_name, width_scale, height_scale) {#int-int-str-int-int}
Fügt der Sammlung ein Bild hinzu.


###  Kehrt zurück

[Picture](/cells/de/python-net/aspose.cells.drawing/picture) Objektindex.


```python
def add(self, upper_left_row, upper_left_column, file_name, width_scale, height_scale):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| upper_left_row | int | Zeilenindex oben links.|
| upper_left_column | int | Spaltenindex oben links.|
| file_name | str | Bilddateiname.|
| width_scale | int | Maßstab der Bildbreite, ein Prozentsatz.|
| height_scale | int | Maßstab der Bildhöhe, ein Prozentsatz.|

###  Beispiel

```python

# add a picture
pictures.add(1, 1, "image.jpg", 50, 50)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [Picture](/cells/de/python-net/aspose.cells.drawing/picture)
* Klasse [PictureCollection](/cells/de/python-net/aspose.cells.drawing/picturecollection)
