---
title: add_group_box Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 110
url: /de/python-net/aspose.cells.drawing/shapecollection/add_group_box/
is_root: false
---
##  add_group_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Fügt dem Arbeitsblatt eine GroupBox hinzu.


###  Kehrt zurück

Ein GroupBox-Objekt.


```python
def add_group_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| upper_left_row | int | Zeilenindex oben links.|
| top | int | Stellt den vertikalen Versatz von GroupBox von seiner linken Zeile in Pixeleinheiten dar.|
| upper_left_column | int | Spaltenindex oben links.|
| left | int | Repräsentiert den horizontalen Versatz von GroupBox von seiner linken Spalte in Pixeleinheiten.|
| height | int | Repräsentiert die Höhe der GroupBox in Pixeleinheiten.|
| width | int | Repräsentiert die Breite der GroupBox in Pixeleinheiten.|

###  Beispiel

```python

# add a group box
groupBox = shapes.add_group_box(1, 0, 1, 0, 100, 50)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection)
