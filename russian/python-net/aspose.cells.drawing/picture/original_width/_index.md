---
title: original_width недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 950
url: /ru/python-net/aspose.cells.drawing/picture/original_width/
is_root: false
---
##  original_width недвижимость

Получает исходную ширину изображения.

###  Пример

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]
# Adding a picture at the location of a cell whose row and column indices are 1 in the worksheet. It is "B2" cell
imgIndex = worksheet.pictures.add(1, 1, "example.jpeg")
# Get the inserted picture object
pic = worksheet.pictures[imgIndex]
# Gets the original width of the picture.
picWidth = pic.original_width
# Save the excel file.
workbook.save("result.xlsx")

```
###  Определение:
```python
@property
def original_width(self):
    ...
```

###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [Picture](/cells/ru/python-net/aspose.cells.drawing/picture)
