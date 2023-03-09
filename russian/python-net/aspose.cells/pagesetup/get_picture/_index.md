---
title: get_picture метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 120
url: /ru/python-net/aspose.cells/pagesetup/get_picture/
is_root: false
---
##  get_picture(is_header, section) {#bool-int}
Получает объект [Picture](/cells/ru/python-net/aspose.cells.drawing/picture) верхнего/нижнего колонтитула.


###  Возвращает

Возвращает объект [Picture](/cells/ru/python-net/aspose.cells.drawing/picture).
Возвращает ноль, если изображения нет.


```python
def get_picture(self, is_header, section):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| is_header | bool | Указывает, находится ли он в верхнем или нижнем колонтитуле.|
| section | int | 0: левая часть, 1: центральная часть, 2: правая часть.|


##  get_picture(is_first, is_even, is_header, section) {#bool-bool-bool-int}
Получает объект [Picture](/cells/ru/python-net/aspose.cells.drawing/picture) верхнего/нижнего колонтитула.


###  Возвращает

Возвращает объект [Picture](/cells/ru/python-net/aspose.cells.drawing/picture).


```python
def get_picture(self, is_first, is_even, is_header, section):
    ...
```


| Параметры| Тип| Описание|
| :- | :- | :- |
| is_first | bool | Указывает, получать ли изображение верхнего/нижнего колонтитула первой страницы.|
| is_even | bool | Указывает, получают ли изображение четного верхнего/нижнего колонтитула страницы.|
| is_header | bool | Указывает, получать ли изображение верхнего/нижнего колонтитула.|
| section | int | 0: левая часть, 1: центральная часть, 2: правая часть.|



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [PageSetup](/cells/ru/python-net/aspose.cells/pagesetup)
* класс [Picture](/cells/ru/python-net/aspose.cells.drawing/picture)
