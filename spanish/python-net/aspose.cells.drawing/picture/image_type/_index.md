---
title: image_type propiedad
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 580
url: /es/python-net/aspose.cells.drawing/picture/image_type/
is_root: false
---
##  image_type propiedad

Obtiene el formato de imagen de la imagen.

###  Ejemplo

```python
from aspose.cells import Workbook
from aspose.cells.drawing import ImageType

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# insert first picture
imgIndex1 = worksheet.pictures.add(1, 1, "1.png")
# Get the inserted picture object
pic1 = worksheet.pictures[imgIndex1]
if pic1.image_type == ImageType.PNG:
    pass
# insert second picture
imgIndex2 = worksheet.pictures.add(1, 9, "2.jpeg")
# Get the inserted picture object
pic2 = worksheet.pictures[imgIndex2]
if pic2.image_type == ImageType.JPEG:
    pass

```
###  Definición:
```python
@property
def image_type(self):
    ...
```

###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [ImageType](/cells/es/python-net/aspose.cells.drawing/imagetype)
* clase [Picture](/cells/es/python-net/aspose.cells.drawing/picture)
