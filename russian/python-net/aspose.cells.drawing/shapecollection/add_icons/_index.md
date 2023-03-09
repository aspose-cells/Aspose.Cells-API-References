---
title: add_icons метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 120
url: /ru/python-net/aspose.cells.drawing/shapecollection/add_icons/
is_root: false
---
##  add_icons(upper_left_row, top, upper_left_column, left, height, width, image_byte_data, compatible_image_data) {#int-int-int-int-int-int-bytes-bytes}
Добавляет SVG-изображение.


###  Возвращает




```python
def add_icons(self, upper_left_row, top, upper_left_column, left, height, width, image_byte_data, compatible_image_data):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| upper_left_row | int | Индекс верхней левой строки.|
| top | int | Представляет вертикальное смещение фигуры от ее левой строки в единицах пикселя.|
| upper_left_column | int |Индекс левого верхнего столбца.|
| left | int | Горизонтальное смещение фигуры от ее левого столбца в пикселях.|
| height | int | Высота фигуры в пикселях.|
| width | int | Ширина фигуры в пикселях.|
| image_byte_data | bytes | Данные байта изображения.|
| compatible_image_data | bytes | Данные изображения преобразованы из svg для совместимости с Excel 2016 или более ранними версиями.|

###  Пример

```python
from aspose import pycore

# add icon
with open("icon.svg", "rb") as fs:
    len = pycore.cast(int, utils.filesize(fs))
    imageData = bytearray(len)
    fs.readinto(imageData)
    picture = shapes.add_svg(4, 0, 5, 0, -1, -1, imageData, None)

```



###  Смотрите также
* модуль [aspose.cells.drawing](../../)
* класс [ShapeCollection](/cells/ru/python-net/aspose.cells.drawing/shapecollection)
