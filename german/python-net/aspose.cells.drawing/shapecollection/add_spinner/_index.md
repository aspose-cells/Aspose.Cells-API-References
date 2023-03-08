---
title: add_spinner Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 290
url: /de/python-net/aspose.cells.drawing/shapecollection/add_spinner/
is_root: false
---
##  add_spinner(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Fügt dem Arbeitsblatt ein Kreisel hinzu.


###  Kehrt zurück

Ein Spinner-Objekt.


```python
def add_spinner(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| upper_left_row | int | Zeilenindex oben links.|
| top | int | Stellt den vertikalen Versatz von Spinner von seiner linken Zeile in Pixeleinheiten dar.|
| upper_left_column | int |Spaltenindex oben links.|
| left | int | Stellt den horizontalen Versatz von Spinner von seiner linken Spalte in Pixeleinheiten dar.|
| height | int | Repräsentiert die Höhe von Spinner in Pixeleinheiten.|
| width | int | Repräsentiert die Breite von Spinner in Pixeleinheiten.|

###  Beispiel

```python

# add a spinner
spinner = shapes.add_spinner(1, 0, 1, 0, 100, 50)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection)
