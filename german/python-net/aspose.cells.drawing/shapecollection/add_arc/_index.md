---
title: add_arc Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 30
url: /de/python-net/aspose.cells.drawing/shapecollection/add_arc/
is_root: false
---
##  add_arc(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Fügt dem Arbeitsblatt eine ArcShape hinzu.


###  Kehrt zurück

Ein ArcShape-Objekt.


```python
def add_arc(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| upper_left_row | int | Zeilenindex oben links.|
| top | int | Stellt den vertikalen Versatz von ArcShape von seiner linken Zeile in Pixeleinheiten dar.|
| upper_left_column | int | Spaltenindex oben links.|
| left | int | Stellt den horizontalen Versatz von ArcShape von seiner linken Spalte in Pixeleinheiten dar.|
| height | int | Stellt die Höhe von ArcShape in Pixeleinheiten dar.|
| width | int |Stellt die Breite von ArcShape in Pixeleinheiten dar.|

###  Beispiele

```python

# add a arc
arcShape = shapes.add_arc(1, 0, 1, 0, 100, 50)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection)
