---
title: add_free_floating_shape método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 100
url: /es/python-net/aspose.cells.drawing/shapecollection/add_free_floating_shape/
is_root: false
---
##  add_free_floating_shape(type, top, left, height, width, image_data, is_original_size) {#MsoDrawingType-int-int-int-int-bytes-bool}
Agrega una forma flotante libre a la hoja de cálculo. Solo se aplica a la forma de línea/imagen.


###  Devoluciones




```python
def add_free_floating_shape(self, type, top, left, height, width, image_data, is_original_size):
    ...
```


| Parámetros| Tipo| Descripción|
| :- | :- | :- |
| type | [MsoDrawingType](/cells/es/python-net/aspose.cells.drawing/msodrawingtype) | El tipo de forma.|
| top | int | Representa el desplazamiento vertical de la forma desde la fila superior de la hoja de cálculo, en unidades de píxel.|
| left | int |Representa el desplazamiento horizontal de la forma desde la columna izquierda de la hoja de cálculo, en unidades de píxel.|
| height | int | Representa la altura de LineShape, en unidades de píxel.|
| width | int | Representa el ancho de LineShape, en unidades de píxel.|
| image_data | bytes | Los datos de la imagen, solo se aplican a la imagen.|
| is_original_size | bool | Si la forma usa el tamaño original si la forma es una imagen.|

###  Ejemplos

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



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ShapeCollection](/cells/es/python-net/aspose.cells.drawing/shapecollection)
