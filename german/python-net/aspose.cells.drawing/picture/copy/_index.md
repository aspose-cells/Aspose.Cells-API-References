---
title: copy Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 60
url: /de/python-net/aspose.cells.drawing/picture/copy/
is_root: false
---
##  copy(source, options) {#Picture-CopyOptions}
Kopieren Sie das Bild.



```python
def copy(self, source, options):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| source | [Picture](/cells/de/python-net/aspose.cells.drawing/picture) | Das Quellbild.|
| options | [CopyOptions](/cells/de/python-net/aspose.cells/copyoptions) | Die Kopieroptionen.|

###  Beispiele

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



###  Siehe auch
* Modul [aspose.cells.drawing](../../)
* Klasse [Picture](/cells/de/python-net/aspose.cells.drawing/picture)
