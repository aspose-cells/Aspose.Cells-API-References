---
title: to_image yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 40
url: /tr/python-net/aspose.cells.rendering/sheetrender/to_image/
is_root: false
---
##  to_image(page_index, file_name) {#int-str}
Belirli bir sayfayı bir dosyaya dönüştürün.



```python
def to_image(self, page_index, file_name):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| page_index | int | hangi sayfanın dönüştürüleceğini belirtin|
| file_name | str | çıktı görüntüsünün dosya adı|

###  Örnek

Aşağıdaki kod, ilk sayfanın ilk sayfasını png görüntüsüne çıkarır.

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
Belirli bir sayfayı bir akışa dönüştürün.



```python
def to_image(self, page_index, stream):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| page_index | int | hangi sayfanın dönüştürüleceğini belirtin|
| stream | io.RawIOBase | çıkış görüntüsünün akışı|



###  Ayrıca bakınız
* modül [aspose.cells.rendering](../../)
* sınıf [SheetRender](/cells/tr/python-net/aspose.cells.rendering/sheetrender)
