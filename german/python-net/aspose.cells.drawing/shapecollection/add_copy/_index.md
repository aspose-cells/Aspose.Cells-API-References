---
title: add_copy Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 90
url: /de/python-net/aspose.cells.drawing/shapecollection/add_copy/
is_root: false
---
##  add_copy(source_shape, upper_left_row, top, upper_left_column, left) {#Shape-int-int-int-int}
Fügt eine Form zum Arbeitsblatt hinzu und kopiert sie.


###  Kehrt zurück

Der neue Formobjektindex.


```python
def add_copy(self, source_shape, upper_left_row, top, upper_left_column, left):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| source_shape | [Shape](/cells/de/python-net/aspose.cells.drawing/shape) | Quellform.|
| upper_left_row | int | Zeilenindex oben links.|
| top | int | Repräsentiert den vertikalen Versatz des Kontrollkästchens von seiner linken Zeile in Pixeleinheiten.|
| upper_left_column | int |Spaltenindex oben links.|
| left | int | Repräsentiert den horizontalen Versatz des Textfelds von seiner linken Spalte in Pixeleinheiten.|

###  Beispiel

```python

# add a shape
rectangle = shapes.add_rectangle(2, 0, 2, 0, 130, 130)
# copy
shapes.add_copy(rectangle, 7, 0, 7, 0)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection)
