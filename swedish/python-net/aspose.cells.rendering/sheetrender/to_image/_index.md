---
title: to_image metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 40
url: /sv/python-net/aspose.cells.rendering/sheetrender/to_image/
is_root: false
---
##  to_image(page_index, file_name) {#int-str}
Gör en viss sida till en fil.



```python
def to_image(self, page_index, file_name):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| page_index | int | ange vilken sida som ska konverteras|
| file_name | str | filnamnet på utdatabilden|

###  Exempel

Följande kod matar ut den första sidan av det första arket till png-bild.

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
Gör en viss sida till en stream.



```python
def to_image(self, page_index, stream):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| page_index | int | ange vilken sida som ska konverteras|
| stream | io.RawIOBase | strömmen av utdatabilden|



###  Se även
* modul [aspose.cells.rendering](../../)
* klass [SheetRender](/cells/sv/python-net/aspose.cells.rendering/sheetrender)
