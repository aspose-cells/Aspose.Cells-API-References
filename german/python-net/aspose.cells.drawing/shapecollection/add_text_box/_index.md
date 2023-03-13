---
title: add_text_box Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 310
url: /de/python-net/aspose.cells.drawing/shapecollection/add_text_box/
is_root: false
---
##  add_text_box(upper_left_row, top, upper_left_column, left, height, width) {#int-int-int-int-int-int}
Fügt dem Arbeitsblatt ein Textfeld hinzu.


###  Kehrt zurück

Ein [TextBox](/cells/de/python-net/aspose.cells.drawing/textbox)-Objekt.


```python
def add_text_box(self, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| upper_left_row | int | Zeilenindex oben links.|
| top | int | Repräsentiert den vertikalen Versatz des Textfelds von seiner linken Zeile in Pixeleinheiten.|
| upper_left_column | int | Spaltenindex oben links.|
| left | int | Repräsentiert den horizontalen Versatz des Textfelds von seiner linken Spalte in Pixeleinheiten.|
| height | int | Repräsentiert die Höhe des Textfelds in Pixeleinheiten.|
| width | int | Repräsentiert die Breite des Textfelds in Pixeleinheiten.|

###  Beispiel

```python

# add a TextBox
textBox = shapes.add_text_box(1, 0, 1, 0, 100, 50)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection)
* Klasse [TextBox](/cells/de/python-net/aspose.cells.drawing/textbox)
