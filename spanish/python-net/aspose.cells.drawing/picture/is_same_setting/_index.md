---
title: is_same_setting método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 140
url: /es/python-net/aspose.cells.drawing/picture/is_same_setting/
is_root: false
---
##  is_same_setting(obj) {#any}
Devuelve si la forma es la misma.


###  Devoluciones




```python
def is_same_setting(self, obj):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| obj | any |  |

###  Ejemplo

```python
from aspose.cells import Workbook

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
if pic1.is_same_setting(pic1):
    pass
if !pic1.is_same_setting(pic2):
    pass

```



###  Ver también
* módulo [aspose.cells.drawing](../../)
* clase [Picture](/cells/es/python-net/aspose.cells.drawing/picture)
