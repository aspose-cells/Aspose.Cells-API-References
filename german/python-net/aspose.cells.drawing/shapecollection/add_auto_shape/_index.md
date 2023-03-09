---
title: add_auto_shape Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 40
url: /de/python-net/aspose.cells.drawing/shapecollection/add_auto_shape/
is_root: false
---
##  add_auto_shape(type, upper_left_row, top, upper_left_column, left, height, width) {#AutoShapeType-int-int-int-int-int-int}
Fügt dem Arbeitsblatt eine AutoForm hinzu.


###  Kehrt zurück

Ein Shape-Objekt.


```python
def add_auto_shape(self, type, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| type | [AutoShapeType](/cells/de/python-net/aspose.cells.drawing/autoshapetype) | Automatischer Formtyp.|
| upper_left_row | int | Zeilenindex oben links.|
| top | int | Stellt den vertikalen Versatz von Shape von seiner linken Zeile in Pixeleinheiten dar.|
| upper_left_column | int | Spaltenindex oben links.|
| left | int | Stellt den horizontalen Versatz von Shape von seiner linken Spalte in Pixeleinheiten dar.|
| height | int | Stellt die Höhe von Shape in Pixeleinheiten dar.|
| width | int | Stellt die Breite von Shape in Pixeleinheiten dar.|
###  Bemerkungen

Der Typ konnte nicht Chart/Comment/Picture/OleObject/Polygon/DialogBox sein
###  Beispiele


```python
from aspose.cells.drawing import AutoShapeType

# Adds a AutoShape to the worksheet.
autoShape = shapes.add_auto_shape(AutoShapeType.CUBE, 1, 0, 1, 0, 100, 50)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection)
