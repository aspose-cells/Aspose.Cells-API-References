---
title: add_oval Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 200
url: /de/python-net/aspose.cells.drawing/shapecollection/add_oval/
is_root: false
---
##  add_oval(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Fügt dem Arbeitsblatt ein Oval hinzu.


###  Kehrt zurück

Ein ovales Objekt.


```python
def add_oval(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| upper_left_row | int | Zeilenindex oben links.|
| top | int | Stellt den vertikalen Versatz von Oval von seiner linken Zeile in Pixeleinheiten dar.|
| upper_left_column | int |Spaltenindex oben links.|
| left | int | Repräsentiert den horizontalen Versatz von Oval von seiner linken Spalte in Pixeleinheiten.|
| height | int | Repräsentiert die Höhe von Oval in Pixeleinheiten.|
| width | int | Repräsentiert die Breite des Ovals in Pixeleinheiten.|

###  Beispiel

```python

# add a oval
oval = shapes.add_oval(1, 0, 1, 0, 50, 50)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection)
