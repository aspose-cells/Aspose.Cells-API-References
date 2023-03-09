---
title: copy método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 60
url: /es/python-net/aspose.cells.drawing/picture/copy/
is_root: false
---
##  copy(source, options) {#Picture-CopyOptions}
Copia la imagen.



```python
def copy(self, source, options):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| source | [Picture](/cells/es/python-net/aspose.cells.drawing/picture) | La imagen fuente.|
| options | [CopyOptions](/cells/es/python-net/aspose.cells/copyoptions) | Las opciones de copia.|

###  Ejemplo

```python
from aspose.cells import CopyOptions, Workbook

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# insert first picture
imgIndex1 = worksheet.pictures.add(1, 1, "1.png")
# Get the inserted picture object
pic1 = worksheet.pictures[imgIndex1]
# insert second picture
imgIndex2 = worksheet.pictures.add(1, 9, "2.jpeg")
# Get the inserted picture object
pic2 = worksheet.pictures[imgIndex2]
# Copy picture 1 to picture 2.You'll get two picture 1 objects that are superimposed on top of each other.
opt = CopyOptions()
pic2.copy(pic1, opt)
# Save the excel file.
workbook.save("result.xlsx")

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [Picture](/cells/es/python-net/aspose.cells.drawing/picture)
