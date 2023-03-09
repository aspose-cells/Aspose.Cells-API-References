---
title: original_height недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 920
url: /ru/python-net/aspose.cells.drawing/picture/original_height/
is_root: false
---
##  original_height недвижимость

Получает исходную высоту изображения.

###  Примеры

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
###  Определение:
```python
@property
def original_height(self):
    ...
```

###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [Picture](/cells/ru/python-net/aspose.cells.drawing/picture)
