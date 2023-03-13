---
title: set_image_resample метод
second_title: Aspose.Cells for Python via .NET API
description:
type: docs
weight: 20
url: /ru/python-net/aspose.cells/pdfsaveoptions/set_image_resample/
is_root: false
---
##  set_image_resample(desired_ppi, jpeg_quality) {#int-int}
 Устанавливает желаемое значение PPI (пикселей на дюйм) изображений с повторной выборкой и качество JPEG.
 Все изображения будут преобразованы в формат JPEG с указанной настройкой качества,
и изображения, которые превышают указанный PPI (пикселей на дюйм), будут передискретизированы.



```python
def set_image_resample(self, desired_ppi, jpeg_quality):
    ...
```


| Параметр| Тип| Описание|
| :- | :- | :- |
| desired_ppi | int | Желаемые пиксели на дюйм. 220 высокого качества. 150 качество экрана. 96 качество электронной почты.|
| jpeg_quality | int | 0 - 100% JPEG качество.|

###  Пример

Следующий код устанавливает желаемый PPI как 96 и качество jpeg как 80 для изображений в выходном PDF-файле.

```python
from aspose.cells import PdfSaveOptions, Workbook

# load the source file with images.
wb = Workbook("Book1.xlsx")
pdfSaveOptions = PdfSaveOptions()
# set desired PPI as 96 and jpeg quality as 80.
pdfSaveOptions.set_image_resample(96, 80)
wb.save("output.pdf", pdfSaveOptions)

```



###  Смотрите также
* модуль [aspose.cells](../../)
* класс [PdfSaveOptions](/cells/ru/python-net/aspose.cells/pdfsaveoptions)
