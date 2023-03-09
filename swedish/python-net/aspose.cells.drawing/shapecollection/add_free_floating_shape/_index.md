---
title: add_free_floating_shape metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 100
url: /sv/python-net/aspose.cells.drawing/shapecollection/add_free_floating_shape/
is_root: false
---
##  add_free_floating_shape(type, top, left, height, width, image_data, is_original_size) {#MsoDrawingType-int-int-int-int-bytes-bool}
Lägger till en fri flytande form till kalkylbladet. Gäller endast linje-/bildform.


###  Returnerar




```python
def add_free_floating_shape(self, type, top, left, height, width, image_data, is_original_size):
    ...
```


| Parametrar| Typ| Beskrivning|
| :- | :- | :- |
| type | [MsoDrawingType](/cells/sv/python-net/aspose.cells.drawing/msodrawingtype) | Formtypen.|
| top | int | Representerar den vertikala förskjutningen av formen från kalkylbladets översta rad, i pixelenhet.|
| left | int |Representerar den horisontella förskjutningen av formen från kalkylbladets vänstra kolumn, i pixelenhet.|
| height | int | Representerar höjden på LineShape, i pixelenhet.|
| width | int | Representerar bredden på LineShape, i pixelenhet.|
| image_data | bytes | Bilddata gäller endast för bilden.|
| is_original_size | bool | Om formen använder originalstorlek om formen är bild.|

###  Exempel

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



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection)
