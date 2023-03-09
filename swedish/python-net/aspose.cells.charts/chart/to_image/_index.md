---
title: to_image metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 120
url: /sv/python-net/aspose.cells.charts/chart/to_image/
is_root: false
---
##  to_image(image_file) {#str}
Skapar diagrambilden och sparar den i en fil.
Förlängningen av filnamnet bestämmer formatet på bilden.



```python
def to_image(self, image_file):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| image_file | str | Bildfilens namn med fullständig sökväg.|
###  Anmärkningar

Bildens format anges med filnamnstillägget.
Till exempel, om du anger "myfile.png", kommer bilden att sparas
 i formatet PNG. Följande filtillägg känns igen:
.bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.


Om bredden eller höjden är noll eller om diagrammet inte stöds enligt listan över stödda diagram, kommer den här metoden inte att göra något.

##  to_image(image_file, image_type) {#str-aspose.cells.drawing.ImageType}
Skapar diagrambilden och sparar den i en fil i angiven bildtyp.



```python
def to_image(self, image_file, image_type):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| image_file | str | Bildfilens namn med fullständig sökväg.|
| image_type | aspose.cells.drawing.ImageType | Bildtypen där bilden ska sparas.|
###  Anmärkningar

Typen av bild anges med `imageType`.
 Följande typer stöds:
ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.


Om bredden eller höjden är noll eller om diagrammet inte stöds enligt listan över stödda diagram, kommer den här metoden inte att göra något.

##  to_image(image_file, jpeg_quality) {#str-int}
Skapar diagrambilden och sparar den i en fil i Jpeg-format.



```python
def to_image(self, image_file, jpeg_quality):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| image_file | str | Bildfilens namn med fullständig sökväg.|
| jpeg_quality | int | Jpeg-kvalitet.|
###  Anmärkningar

Om bredden eller höjden är noll eller om diagrammet inte stöds enligt listan över stödda diagram, kommer den här metoden inte att göra något.

##  to_image(stream, jpeg_quality) {#io.RawIOBase-int}

Skapar diagrambilden och sparar den i en ström i Jpeg-format.



```python
def to_image(self, stream, jpeg_quality):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| stream | io.RawIOBase | Utgångsströmmen.|
| jpeg_quality | int | Jpeg-kvalitet.|
###  Anmärkningar

Om bredden eller höjden är noll eller om diagrammet inte stöds enligt listan över stödda diagram, kommer den här metoden inte att göra något.

##  to_image(stream, image_type) {#io.RawIOBase-aspose.cells.drawing.ImageType}

Skapar diagrambilden och sparar den i en ström i det angivna formatet.



```python
def to_image(self, stream, image_type):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| stream | io.RawIOBase | Utgångsströmmen.|
| image_type | aspose.cells.drawing.ImageType | Bildtypen där bilden ska sparas.|
###  Anmärkningar

Typen av bild anges med `imageType`.
 Följande typer stöds:
ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.


Om bredden eller höjden är noll eller om diagrammet inte stöds enligt listan över stödda diagram, kommer den här metoden inte att göra något.

##  to_image(image_file, options) {#str-aspose.cells.rendering.ImageOrPrintOptions}
Skapar diagrambilden och sparar den i en fil.
Förlängningen av filnamnet bestämmer formatet på bilden.



```python
def to_image(self, image_file, options):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| image_file | str | Bildfilens namn med fullständig sökväg.|
| options | aspose.cells.rendering.ImageOrPrintOptions | Ytterligare bildskapande alternativ|
###  Anmärkningar

Bildens format anges med filnamnstillägget.
Till exempel, om du anger "myfile.png", kommer bilden att sparas
 i formatet PNG. Följande filtillägg känns igen:
.bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.


Om bredden eller höjden är noll eller om diagrammet inte stöds enligt listan över stödda diagram, kommer den här metoden inte att göra något.
 Vänligen hänvisa till[Sjökortslista som stöds](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) för mer detaljer.
###  Exempel

Sparar till Tiff med 300 dpi och CCITT4-komprimering.

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions, TiffCompression

options = ImageOrPrintOptions()
options.horizontal_resolution = 300
options.vertical_resolution = 300
options.tiff_compression = TiffCompression.COMPRESSION_CCITT4
book = Workbook(r"test.xls")
book.worksheets[0].charts[0].to_image(r"chart.Tiff", options)

```


Sparar till Jpeg med 300 dpi och 80 bildkvalitet.

```python
from aspose.cells import Workbook
from aspose.cells.rendering import ImageOrPrintOptions

options = ImageOrPrintOptions()
options.horizontal_resolution = 300
options.vertical_resolution = 300
options.quality = 80
book = Workbook(r"test.xls")
book.worksheets[0].charts[0].to_image(r"chart.Jpeg", options)

```


##  to_image(stream, options) {#io.RawIOBase-aspose.cells.rendering.ImageOrPrintOptions}
Skapar diagrambilden och sparar den i en ström i det angivna formatet.



```python
def to_image(self, stream, options):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| stream | io.RawIOBase | Utgångsströmmen.|
| options | aspose.cells.rendering.ImageOrPrintOptions | Ytterligare bildskapande alternativ|
###  Anmärkningar

Typen av bild anges med `options.ImageType`.
Följande format stöds:
ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.


Om bredden eller höjden är noll eller om diagrammet inte stöds enligt listan över stödda diagram, kommer den här metoden inte att göra något.
 Vänligen hänvisa till[Sjökortslista som stöds](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) för mer detaljer.


###  Se även
* modul [aspose.cells.charts](../../)
* klass [Chart](/cells/sv/python-net/aspose.cells.charts/chart)
