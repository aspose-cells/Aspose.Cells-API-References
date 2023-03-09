---
title: add_radio_button Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 230
url: /de/python-net/aspose.cells.drawing/shapecollection/add_radio_button/
is_root: false
---
##  add_radio_button(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Fügt dem Arbeitsblatt einen RadioButton hinzu.


###  Kehrt zurück

Ein RadioButton-Objekt.


```python
def add_radio_button(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| upper_left_row | int | Zeilenindex oben links.|
| top | int | Stellt den vertikalen Abstand von RadioButton von seiner linken Zeile in Pixeleinheiten dar.|
| upper_left_column | int | Spaltenindex oben links.|
| left | int | Stellt den horizontalen Versatz von RadioButton von seiner linken Spalte in Pixeleinheiten dar.|
| height | int | Repräsentiert die Höhe von RadioButton in Pixeleinheiten.|
| width | int | Repräsentiert die Breite von RadioButton in Pixeleinheiten.|

###  Beispiele

```python

# add a radio button
radioButton = shapes.add_radio_button(1, 0, 1, 0, 100, 50)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection)
