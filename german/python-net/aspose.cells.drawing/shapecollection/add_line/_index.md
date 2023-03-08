---
title: add_line Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 150
url: /de/python-net/aspose.cells.drawing/shapecollection/add_line/
is_root: false
---
##  add_line(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Fügt dem Arbeitsblatt eine Linienform hinzu.


###  Kehrt zurück

Ein LineShape-Objekt.


```python
def add_line(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| upper_left_row | int | Zeilenindex oben links.|
| top | int | Stellt den vertikalen Versatz von LineShape von seiner linken Zeile in Pixeleinheiten dar.|
| upper_left_column | int |Spaltenindex oben links.|
| left | int | Repräsentiert den horizontalen Versatz von LineShape von seiner linken Spalte in Pixeleinheiten.|
| height | int | Repräsentiert die Höhe von LineShape in Pixeleinheiten.|
| width | int | Repräsentiert die Breite von LineShape in Pixeleinheiten.|

###  Beispiel

```python

#  add a line object
lineShape = shapes.add_line(1, 0, 1, 0, 100, 50)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection)
