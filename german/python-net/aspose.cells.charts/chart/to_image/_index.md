---
title: to_image Methode
second_title: Aspose.Cells for Python via .NET API Referenzen
description:
type: docs
weight: 120
url: /de/python-net/aspose.cells.charts/chart/to_image/
is_root: false
---
##  to_image(image_file) {#str}
Erstellt das Diagrammbild und speichert es in einer Datei.
Die Erweiterung des Dateinamens bestimmt das Format des Bildes.



```python
def to_image(self, image_file):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| image_file | str | Der Bilddateiname mit vollständigem Pfad.|
###  Bemerkungen

Das Format des Bildes wird durch die Erweiterung des Dateinamens angegeben.
Wenn Sie beispielsweise „myfile.png“ angeben, wird das Bild gespeichert
 im Format PNG. Die folgenden Dateierweiterungen werden erkannt:
.bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.


Wenn die Breite oder Höhe Null ist oder das Diagramm gemäß der Liste der unterstützten Diagramme nicht unterstützt wird, wird diese Methode nichts bewirken.

##  to_image(image_file, image_type) {#str-aspose.cells.drawing.ImageType}
Erstellt das Diagrammbild und speichert es in einer Datei im angegebenen Bildtyp.



```python
def to_image(self, image_file, image_type):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| image_file | str | Der Bilddateiname mit vollständigem Pfad.|
| image_type | aspose.cells.drawing.ImageType | Der Bildtyp, in dem das Bild gespeichert werden soll.|
###  Bemerkungen

Der Typ des Bildes wird mit `imageType` angegeben.
 Die folgenden Typen werden unterstützt:
ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.


Wenn die Breite oder Höhe Null ist oder das Diagramm gemäß der Liste der unterstützten Diagramme nicht unterstützt wird, wird diese Methode nichts bewirken.

##  to_image(image_file, jpeg_quality) {#str-int}
Erstellt das Diagrammbild und speichert es in einer Datei im JPEG-Format.



```python
def to_image(self, image_file, jpeg_quality):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| image_file | str | Der Bilddateiname mit vollständigem Pfad.|
| jpeg_quality | int | JPEG-Qualität.|
###  Bemerkungen

Wenn die Breite oder Höhe Null ist oder das Diagramm gemäß der Liste der unterstützten Diagramme nicht unterstützt wird, wird diese Methode nichts bewirken.

##  to_image(stream, jpeg_quality) {#io.RawIOBase-int}

Erstellt das Diagrammbild und speichert es in einem Stream im JPEG-Format.



```python
def to_image(self, stream, jpeg_quality):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| stream | io.RawIOBase | Der Ausgangsstrom.|
| jpeg_quality | int | JPEG-Qualität.|
###  Bemerkungen

Wenn die Breite oder Höhe Null ist oder das Diagramm gemäß der Liste der unterstützten Diagramme nicht unterstützt wird, wird diese Methode nichts bewirken.

##  to_image(stream, image_type) {#io.RawIOBase-aspose.cells.drawing.ImageType}

Erstellt das Diagrammbild und speichert es im angegebenen Format in einem Stream.



```python
def to_image(self, stream, image_type):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| stream | io.RawIOBase | Der Ausgangsstrom.|
| image_type | aspose.cells.drawing.ImageType | Der Bildtyp, in dem das Bild gespeichert werden soll.|
###  Bemerkungen

Der Typ des Bildes wird mit `imageType` angegeben.
 Die folgenden Typen werden unterstützt:
ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.


Wenn die Breite oder Höhe Null ist oder das Diagramm gemäß der Liste der unterstützten Diagramme nicht unterstützt wird, wird diese Methode nichts bewirken.

##  to_image(image_file, options) {#str-aspose.cells.rendering.ImageOrPrintOptions}
Erstellt das Diagrammbild und speichert es in einer Datei.
Die Erweiterung des Dateinamens bestimmt das Format des Bildes.



```python
def to_image(self, image_file, options):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| image_file | str | Der Bilddateiname mit vollständigem Pfad.|
| options | aspose.cells.rendering.ImageOrPrintOptions | Zusätzliche Bilderzeugungsoptionen|
###  Bemerkungen

Das Format des Bildes wird durch die Erweiterung des Dateinamens angegeben.
Wenn Sie beispielsweise „myfile.png“ angeben, wird das Bild gespeichert
 im Format PNG. Die folgenden Dateierweiterungen werden erkannt:
.bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.


Wenn die Breite oder Höhe Null ist oder das Diagramm gemäß der Liste der unterstützten Diagramme nicht unterstützt wird, wird diese Methode nichts bewirken.
 Bitte beziehen Sie sich auf[Liste der unterstützten Diagramme](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html)für mehr Details.
###  Beispiel

Speichert im Tiff-Format mit 300 dpi und CCITT4-Komprimierung.

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


Speichert als JPEG mit 300 dpi und 80 Bildqualität.

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
Erstellt das Diagrammbild und speichert es im angegebenen Format in einem Stream.



```python
def to_image(self, stream, options):
    ...
```


| Parameter| Typ| Beschreibung|
| :- | :- | :- |
| stream | io.RawIOBase | Der Ausgangsstrom.|
| options | aspose.cells.rendering.ImageOrPrintOptions | Zusätzliche Bilderzeugungsoptionen|
###  Bemerkungen

Der Typ des Bildes wird mit `options.ImageType` angegeben.
 Folgende Formate werden unterstützt:
ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.


Wenn die Breite oder Höhe Null ist oder das Diagramm gemäß der Liste der unterstützten Diagramme nicht unterstützt wird, wird diese Methode nichts bewirken.
 Bitte beziehen Sie sich auf[Liste der unterstützten Diagramme](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html)für mehr Details.


###  Siehe auch
* Modul [aspose.cells.charts](../../)
* Klasse [Chart](/cells/de/python-net/aspose.cells.charts/chart)
