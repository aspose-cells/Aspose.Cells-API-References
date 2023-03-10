---
title: add_free_floating_shape Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 100
url: /de/python-net/aspose.cells.drawing/shapecollection/add_free_floating_shape/
is_root: false
---
##  add_free_floating_shape(type, top, left, height, width, image_data, is_original_size) {#MsoDrawingType-int-int-int-int-bytes-bool}
Fügt dem Arbeitsblatt eine freischwebende Form hinzu. Gilt nur für Linien-/Bildform.


###  Kehrt zurück




```python
def add_free_floating_shape(self, type, top, left, height, width, image_data, is_original_size):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| type | [MsoDrawingType](/cells/de/python-net/aspose.cells.drawing/msodrawingtype) | Der Formtyp.|
| top | int | Stellt den vertikalen Versatz der Form von der obersten Zeile des Arbeitsblatts in Pixeleinheiten dar.|
| left | int |Stellt den horizontalen Versatz der Form von der linken Spalte des Arbeitsblatts in Pixeleinheiten dar.|
| height | int | Repräsentiert die Höhe von LineShape in Pixeleinheiten.|
| width | int | Repräsentiert die Breite von LineShape in Pixeleinheiten.|
| image_data | bytes | Die Bilddaten gelten nur für das Bild.|
| is_original_size | bool | Ob die Form die Originalgröße verwendet, wenn es sich bei der Form um ein Bild handelt.|

###  Beispiel

```python
from aspose import pycore
from aspose.cells.drawing import MsoDrawingType

# add a line
floatingShape_Line = shapes.add_free_floating_shape(MsoDrawingType.LINE, 100, 100, 100, 50, None, False)
# add a picture
imageData = None
with open("image.jpg", "rb") as fs:
    len = pycore.cast(int, utils.filesize(fs))
    imageData = bytearray(len)
    fs.readinto(imageData)
floatingShape_Picture = shapes.add_free_floating_shape(MsoDrawingType.PICTURE, 200, 100, 100, 50, imageData, False)

```



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [ShapeCollection](/cells/de/python-net/aspose.cells.drawing/shapecollection)
