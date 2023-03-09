---
title: set_picture метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 220
url: /ru/python-net/aspose.cells/pagesetup/set_picture/
is_root: false
---
##  set_picture(is_first, is_even, is_header, section, image_data) {#bool-bool-bool-int-bytes}
Устанавливает изображение в верхний/нижний колонтитул листа.


###  Возвращает

Возвращает объект [Picture](/cells/ru/python-net/aspose.cells.drawing/picture).


```python
def set_picture(self, is_first, is_even, is_header, section, image_data):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| is_first | bool | Указывает, устанавливается ли изображение верхнего/нижнего колонтитула первой страницы.|
| is_even | bool | Указывает, устанавливается ли изображение четного верхнего/нижнего колонтитула страницы.|
| is_header | bool | Указывает, устанавливается ли изображение верхнего/нижнего колонтитула.|
| section | int | 0: левая часть, 1: центральная часть, 2: правая часть.|
| image_data | bytes | Данные изображения.|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [PageSetup](/cells/ru/python-net/aspose.cells/pagesetup)
* класс [Picture](/cells/ru/python-net/aspose.cells.drawing/picture)
