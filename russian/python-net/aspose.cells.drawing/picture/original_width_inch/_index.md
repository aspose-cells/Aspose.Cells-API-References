---
title: original_width_inch недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 970
url: /ru/python-net/aspose.cells.drawing/picture/original_width_inch/
is_root: false
---
##  original_width_inch недвижимость

Получает исходную ширину изображения в дюймах.

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
picWidthInch = pic.original_width_inch
# Save the excel file.
workbook.save("result.xlsx")

```
###  Определение:
```python
@property
def original_width_inch(self):
    ...
```

###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [Picture](/cells/ru/python-net/aspose.cells.drawing/picture)
