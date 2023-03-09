---
title: to_image метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 40
url: /ru/python-net/aspose.cells.rendering/sheetrender/to_image/
is_root: false
---
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

###  Пример

Следующий код выводит первую страницу первого листа в изображение png.

```python
from aspose.cells import Workbook
from aspose.cells.drawing import ImageType
from aspose.cells.rendering import ImageOrPrintOptions, SheetRender

# load the source file with images.
wb = Workbook("Book1.xlsx")
imgOpt = ImageOrPrintOptions()
# set output image type.
imgOpt.image_type = ImageType.PNG
# render the first sheet.
sr = SheetRender(wb.worksheets[0], imgOpt)
# output the first page of the sheet to image.
sr.to_image(0, "output.png")

```


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
* класс [SheetRender](/cells/ru/python-net/aspose.cells.rendering/sheetrender)
