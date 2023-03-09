---
title: metodo add_free_floating_shape
second_title: Aspose.Cells for Python via .NET API Referenze
description:
type: docs
weight: 100
url: /it/python-net/aspose.cells.drawing/shapecollection/add_free_floating_shape/
is_root: false
---
##  add_free_floating_shape(type, top, left, height, width, image_data, is_original_size) {#MsoDrawingType-int-int-int-int-bytes-bool}
Aggiunge una forma fluttuante libera al foglio di lavoro. Si applica solo alla forma linea/immagine.


###  ritorna




```python
def add_free_floating_shape(self, type, top, left, height, width, image_data, is_original_size):
    ...
```


| Parametro| Tipo| Descrizione|
| :- | :- | :- |
| type | [MsoDrawingType](/cells/it/python-net/aspose.cells.drawing/msodrawingtype) | Il tipo di forma.|
| top | int |Rappresenta l'offset verticale della forma dalla riga superiore del foglio di lavoro, in unità di pixel.|
| left | int | Rappresenta l'offset orizzontale della forma dalla colonna sinistra del foglio di lavoro, in unità di pixel.|
| height | int | Rappresenta l'altezza di LineShape, in unità di pixel.|
| width | int | Rappresenta la larghezza di LineShape, in unità di pixel.|
| image_data | bytes | I dati dell'immagine si applicano solo all'immagine.|
| is_original_size | bool | Se la forma usa la dimensione originale se la forma è un'immagine.|

###  Esempio

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



###  Guarda anche
* modulo [aspose.cells.drawing](../../)
* classe [ShapeCollection](/cells/it/python-net/aspose.cells.drawing/shapecollection)
