---
title: add_icons metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 120
url: /sv/python-net/aspose.cells.drawing/shapecollection/add_icons/
is_root: false
---
##  add_icons(upper_left_row, top, upper_left_column, left, height, width, image_byte_data, compatible_image_data) {#int-int-int-int-int-int-bytes-bytes}
Lägger till svg-bild.


###  Returnerar




```python
def add_icons(self, upper_left_row, top, upper_left_column, left, height, width, image_byte_data, compatible_image_data):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| upper_left_row | int | Övre vänstra radens index.|
| top | int | Representerar den vertikala förskjutningen av formen från dess vänstra rad, i pixelenhet.|
| upper_left_column | int | Övre vänstra kolumnindex.|
| left | int | Den horisontella förskjutningen av formen från dess vänstra kolumn, i pixelenhet.|
| height | int | Formens höjd, i pixelenhet.|
| width | int | Formens bredd, i pixelenhet.|
| image_byte_data | bytes | Bildbytedata.|
| compatible_image_data | bytes |Konverterade bilddata från svg för att vara kompatibel med Excel 2016 eller lägre versioner.|

###  Exempel

```python
from aspose import pycore

# add icon
with open("icon.svg", "rb") as fs:
    len = pycore.cast(int, utils.filesize(fs))
    imageData = bytearray(len)
    fs.readinto(imageData)
    picture = shapes.add_svg(4, 0, 5, 0, -1, -1, imageData, None)

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [ShapeCollection](/cells/sv/python-net/aspose.cells.drawing/shapecollection)
