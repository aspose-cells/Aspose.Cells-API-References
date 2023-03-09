---
title: add_free_floating_shape метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 100
url: /ru/python-net/aspose.cells.drawing/shapecollection/add_free_floating_shape/
is_root: false
---
##  add_free_floating_shape(type, top, left, height, width, image_data, is_original_size) {#MsoDrawingType-int-int-int-int-bytes-bool}
Добавляет на лист свободно плавающую фигуру. Применяется только для формы линии/изображения.


###  Возвращает




```python
def add_free_floating_shape(self, type, top, left, height, width, image_data, is_original_size):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| type | [MsoDrawingType](/cells/ru/python-net/aspose.cells.drawing/msodrawingtype) | Тип формы.|
| top | int |Представляет вертикальное смещение фигуры от верхней строки рабочего листа в единицах пикселя.|
| left | int | Представляет горизонтальное смещение фигуры от левого столбца рабочего листа в пикселях.|
| height | int | Представляет высоту LineShape в пикселях.|
| width | int | Представляет ширину LineShape в пикселях.|
| image_data | bytes | Данные изображения относятся только к изображению.|
| is_original_size | bool | Использует ли фигура исходный размер, если фигура является изображением.|

###  Пример

```python
from aspose import pycore
from aspose.cells.drawing import MsoDrawingType

# add a line
floatingShape_Line = shapes.add_free_floating_shape(MsoDrawingType.LINE, 100, 100, 100, 50, None, False)
# add a picture
imageData = None
with open("image.jpg", "rb") as fs:
    len = pycore.cast(int, utils.filesize(fs))
    imageData = bytearray(len)
    fs.readinto(imageData)
floatingShape_Picture = shapes.add_free_floating_shape(MsoDrawingType.PICTURE, 200, 100, 100, 50, imageData, False)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)
