---
title: add_check_box Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 70
url: /de/python-net/aspose.cells.drawing/shapecollection/add_check_box/
is_root: false
---
##  add_check_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Fügt dem Arbeitsblatt ein Kontrollkästchen hinzu.


###  Kehrt zurück

Der neue CheckBox-Objektindex.


```python
def add_check_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| upper_left_row | int | Zeilenindex oben links.|
| top | int |Repräsentiert den vertikalen Versatz des Kontrollkästchens von seiner linken Zeile in Pixeleinheiten.|
| upper_left_column | int | Spaltenindex oben links.|
| left | int | Repräsentiert den horizontalen Versatz des Textfelds von seiner linken Spalte in Pixeleinheiten.|
| height | int | Höhe des Textfelds in Pixeleinheiten.|
| width | int | Breite des Textfelds in Pixeleinheiten.|

###  Beispiele

```python

# add a CheckBox
checkBox = shapes.add_check_box(1, 0, 1, 0, 100, 50)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection)
