---
title: to_tiff metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 60
url: /sv/python-net/aspose.cells.rendering/sheetrender/to_tiff/
is_root: false
---
##  to_tiff(stream) {#io.RawIOBase}
Gör hela kalkylbladet som Tiff-bild för att streama.



```python
def to_tiff(self, stream):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| stream | io.RawIOBase | strömmen av utdatabilden|


##  to_tiff(filename) {#str}
Gör hela kalkylbladet som Tiff-bild till en fil.



```python
def to_tiff(self, filename):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| filename | str | filnamnet på utdatabilden|

###  Exempel

Följande kod matar ut alla sidorna i det första arket till Tiff-bild.

```python
from aspose.cells import SaveFormat, Workbook
from aspose.cells.rendering import ImageOrPrintOptions, SheetRender

# load the source file with images.
wb = Workbook("Book1.xlsx")
imgOpt = ImageOrPrintOptions()
# set output image type.
imgOpt.save_format = SaveFormat.TIFF
# render the first sheet.
sr = SheetRender(wb.worksheets[0], imgOpt)
# output all the pages of the sheet to Tiff image.
sr.to_tiff("output.tiff")

```



###  Se även
* modul [aspose.cells.rendering](../../)
* klass [SheetRender](/cells/sv/python-net/aspose.cells.rendering/sheetrender)
