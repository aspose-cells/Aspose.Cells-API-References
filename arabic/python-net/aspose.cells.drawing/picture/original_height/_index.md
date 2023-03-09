---
title: original_height الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 920
url: /ar/python-net/aspose.cells.drawing/picture/original_height/
is_root: false
---
##  original_height الملكية

الحصول على الارتفاع الأصلي للصورة.

###  أمثلة

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
imgIndex = worksheet.pictures.add(1, 1, "example.jpeg")
# Get the inserted picture object
pic = worksheet.pictures[imgIndex]
# Gets the original height of the picture.
picHeight = pic.original_height
# Save the excel file.
workbook.save("result.xlsx")

```
###  تعريف:
```python
@property
def original_height(self):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [Picture](/cells/ar/python-net/aspose.cells.drawing/picture)
