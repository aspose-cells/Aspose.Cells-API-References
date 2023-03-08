---
title: add_rectangle Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 240
url: /de/python-net/aspose.cells.drawing/shapecollection/add_rectangle/
is_root: false
---
##  add_rectangle(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Fügt dem Arbeitsblatt ein RectangleShape hinzu.


###  Kehrt zurück

Ein RectangleShape-Objekt.


```python
def add_rectangle(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| upper_left_row | int | Zeilenindex oben links.|
| top | int | Stellt den vertikalen Versatz von RectangleShape von seiner linken Zeile in Pixeleinheiten dar.|
| upper_left_column | int |Spaltenindex oben links.|
| left | int | Stellt den horizontalen Versatz von RectangleShape von seiner linken Spalte in Pixeleinheiten dar.|
| height | int | Stellt die Höhe von RectangleShape in Pixeleinheiten dar.|
| width | int | Stellt die Breite von RectangleShape in Pixeleinheiten dar.|

###  Beispiel

```python

#  add a rectangle
rectangleShape = shapes.add_rectangle(2, 0, 2, 0, 130, 130)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection)
