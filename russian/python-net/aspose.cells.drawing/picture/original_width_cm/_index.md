---
title: original_width_cm недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 960
url: /ru/python-net/aspose.cells.drawing/picture/original_width_cm/
is_root: false
---
##  original_width_cm недвижимость

Получает исходную ширину изображения в сантиметрах.

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
picWidthCM = pic.original_width_cm
# Save the excel file.
workbook.save("result.xlsx")

```
###  Определение:
```python
@property
def original_width_cm(self):
    ...
```

###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [Picture](/cells/ru/python-net/aspose.cells.drawing/picture)
