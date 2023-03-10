---
title: add_svg Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 300
url: /de/python-net/aspose.cells.drawing/shapecollection/add_svg/
is_root: false
---
##  add_svg(upper_left_row, top, upper_left_column, left, height, width, svg_data, compatible_image_data) {#int-int-int-int-int-int-bytes-bytes}
Fügt ein SVG-Bild hinzu.


###  Kehrt zurück




```python
def add_svg(self, upper_left_row, top, upper_left_column, left, height, width, svg_data, compatible_image_data):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| upper_left_row | int | Zeilenindex oben links.|
| top | int | Stellt den vertikalen Versatz der Form von der linken Zeile in Pixeleinheiten dar.|
| upper_left_column | int | Spaltenindex oben links.|
| left | int | Der horizontale Versatz der Form von der linken Spalte in Pixeleinheiten.|
| height | int | Die Höhe der Form in Pixeleinheiten.|
| width | int | Die Breite der Form in Pixeleinheiten.|
| svg_data | bytes | Die SVG-Bilddaten.|
| compatible_image_data | bytes |Konvertierte Bilddaten von svg, um mit Excel 2016 oder niedrigeren Versionen kompatibel zu sein.|

###  Beispiel

```python
from aspose import pycore

#  add a svg
with open("image.svg", "rb") as fs:
    len = pycore.cast(int, utils.filesize(fs))
    imageData = bytearray(len)
    fs.readinto(imageData)
    picture = shapes.add_svg(4, 0, 5, 0, -1, -1, imageData, None)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection)
