---
title: metodo add_svg
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 300
url: /it/python-net/aspose.cells.drawing/shapecollection/add_svg/
is_root: false
---
##  add_svg(upper_left_row, top, upper_left_column, left, height, width, svg_data, compatible_image_data) {#int-int-int-int-int-int-bytes-bytes}
Aggiunge un'immagine svg.


###  ritorna




```python
def add_svg(self, upper_left_row, top, upper_left_column, left, height, width, svg_data, compatible_image_data):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| upper_left_row | int | Indice della riga in alto a sinistra.|
| top | int | Rappresenta l'offset verticale della forma dalla riga sinistra, in unità di pixel.|
| upper_left_column | int | Indice colonna in alto a sinistra.|
| left | int | L'offset orizzontale della forma dalla sua colonna di sinistra, in unità di pixel.|
| height | int | L'altezza della forma, in unità di pixel.|
| width | int | La larghezza della forma, in unità di pixel.|
| svg_data | bytes | I dati dell'immagine svg.|
| compatible_image_data | bytes |Dati di immagine convertiti da svg per essere compatibili con Excel 2016 o versioni precedenti.|

###  Esempio

```python
from aspose import pycore

#  add a svg
with open("image.svg", "rb") as fs:
    len = pycore.cast(int, utils.filesize(fs))
    imageData = bytearray(len)
    fs.readinto(imageData)
    picture = shapes.add_svg(4, 0, 5, 0, -1, -1, imageData, None)

```



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)
