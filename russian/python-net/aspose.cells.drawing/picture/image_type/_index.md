---
title: image_type недвижимость
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 580
url: /ru/python-net/aspose.cells.drawing/picture/image_type/
is_root: false
---
##  image_type недвижимость

Получает формат изображения изображения.

###  Пример

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
###  Определение:
```python
@property
def image_type(self):
    ...
```

###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ImageType](/cells/ru/python-net/aspose.cells.drawing/imagetype)
* класс [Picture](/cells/ru/python-net/aspose.cells.drawing/picture)
