---
title: to_image метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 40
url: /ru/python-net/aspose.cells.rendering/workbookrender/to_image/
is_root: false
---
##  to_image(stream) {#io.RawIOBase}
Рендеринг всей книги в виде изображения Tiff для потоковой передачи.



```python
def to_image(self, stream):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| stream | io.RawIOBase | поток выходного изображения|


##  to_image(filename) {#str}
Визуализация всей книги в виде изображения Tiff в файл.



```python
def to_image(self, filename):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| filename | str | имя файла выходного изображения|


##  to_image(page_index, file_name) {#int-str}
Рендерить определенную страницу в файл.



```python
def to_image(self, page_index, file_name):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| page_index | int | указать, какая страница должна быть преобразована|
| file_name | str | имя файла выходного изображения|


##  to_image(page_index, stream) {#int-io.RawIOBase}
Рендерить определенную страницу в поток.



```python
def to_image(self, page_index, stream):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| page_index | int | указать, какая страница должна быть преобразована|
| stream | io.RawIOBase | поток выходного изображения|



###  Смотрите также
* модуль [aspose.cells.rendering](../../)
* класс [WorkbookRender](/cells/ru/python-net/aspose.cells.rendering/workbookrender)
