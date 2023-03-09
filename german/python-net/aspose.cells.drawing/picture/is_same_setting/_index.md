---
title: is_same_setting Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 140
url: /de/python-net/aspose.cells.drawing/picture/is_same_setting/
is_root: false
---
##  is_same_setting(obj) {#any}
Gibt zurück, ob die Form gleich ist.


###  Kehrt zurück




```python
def is_same_setting(self, obj):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| obj | any |  |

###  Beispiele

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



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [Picture](/cells/de/python-net/aspose.cells.drawing/picture)
