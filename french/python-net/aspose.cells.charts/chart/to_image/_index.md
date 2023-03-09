---
title: to_image méthode
second_title: Aspose.Cells for Python via .NET API Références
description:
type: docs
weight: 120
url: /fr/python-net/aspose.cells.charts/chart/to_image/
is_root: false
---
##  to_image(image_file) {#str}
Crée l'image du graphique et l'enregistre dans un fichier.
L'extension du nom de fichier détermine le format de l'image.



```python
def to_image(self, image_file):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| image_file | str | Le nom du fichier image avec le chemin complet.|
###  Remarques

Le format de l'image est spécifié en utilisant l'extension du nom de fichier.
Par exemple, si vous spécifiez "monfichier.png", l'image sera enregistrée
 au format PNG. Les extensions de fichier suivantes sont reconnues :
.bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.


Si la largeur ou la hauteur est nulle ou si le graphique n'est pas pris en charge conformément à la liste des graphiques pris en charge, cette méthode ne fera rien.

##  to_image(image_file, image_type) {#str-aspose.cells.drawing.ImageType}
Crée l'image du graphique et l'enregistre dans un fichier dans le type d'image spécifié.



```python
def to_image(self, image_file, image_type):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| image_file | str | Le nom du fichier image avec le chemin complet.|
| image_type | aspose.cells.drawing.ImageType | Type d'image dans lequel enregistrer l'image.|
###  Remarques

Le type d'image est spécifié à l'aide de `imageType`.
 Les types suivants sont pris en charge :
ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.


Si la largeur ou la hauteur est nulle ou si le graphique n'est pas pris en charge conformément à la liste des graphiques pris en charge, cette méthode ne fera rien.

##  to_image(image_file, jpeg_quality) {#str-int}
Crée l'image du graphique et l'enregistre dans un fichier au format Jpeg.



```python
def to_image(self, image_file, jpeg_quality):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| image_file | str | Le nom du fichier image avec le chemin complet.|
| jpeg_quality | int | Qualité Jpeg.|
###  Remarques

Si la largeur ou la hauteur est nulle ou si le graphique n'est pas pris en charge conformément à la liste des graphiques pris en charge, cette méthode ne fera rien.

##  to_image(stream, jpeg_quality) {#io.RawIOBase-int}

Crée l'image du graphique et l'enregistre dans un flux au format Jpeg.



```python
def to_image(self, stream, jpeg_quality):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| stream | io.RawIOBase | Le flux de sortie.|
| jpeg_quality | int | Qualité Jpeg.|
###  Remarques

Si la largeur ou la hauteur est nulle ou si le graphique n'est pas pris en charge conformément à la liste des graphiques pris en charge, cette méthode ne fera rien.

##  to_image(stream, image_type) {#io.RawIOBase-aspose.cells.drawing.ImageType}

Crée l'image du graphique et l'enregistre dans un flux au format spécifié.



```python
def to_image(self, stream, image_type):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| stream | io.RawIOBase | Le flux de sortie.|
| image_type | aspose.cells.drawing.ImageType | Type d'image dans lequel enregistrer l'image.|
###  Remarques

Le type d'image est spécifié à l'aide de `imageType`.
 Les types suivants sont pris en charge :
ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.


Si la largeur ou la hauteur est nulle ou si le graphique n'est pas pris en charge conformément à la liste des graphiques pris en charge, cette méthode ne fera rien.

##  to_image(image_file, options) {#str-aspose.cells.rendering.ImageOrPrintOptions}
Crée l'image du graphique et l'enregistre dans un fichier.
L'extension du nom de fichier détermine le format de l'image.



```python
def to_image(self, image_file, options):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| image_file | str | Le nom du fichier image avec le chemin complet.|
| options | aspose.cells.rendering.ImageOrPrintOptions | Options de création d'images supplémentaires|
###  Remarques

Le format de l'image est spécifié en utilisant l'extension du nom de fichier.
Par exemple, si vous spécifiez "monfichier.png", l'image sera enregistrée
 au format PNG. Les extensions de fichier suivantes sont reconnues :
.bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.


Si la largeur ou la hauteur est nulle ou si le graphique n'est pas pris en charge conformément à la liste des graphiques pris en charge, cette méthode ne fera rien.
 Prière de se référer à[Liste des graphiques pris en charge](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) pour plus de détails.
###  Exemple

Enregistre au format Tiff avec 300 dpi et compression CCITT4.

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


Enregistre au format Jpeg avec une résolution de 300 dpi et une qualité d'image de 80.

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
Crée l'image du graphique et l'enregistre dans un flux au format spécifié.



```python
def to_image(self, stream, options):
    ...
```


| Paramètre| Taper| Description|
| :- | :- | :- |
| stream | io.RawIOBase | Le flux de sortie.|
| options | aspose.cells.rendering.ImageOrPrintOptions | Options de création d'images supplémentaires|
###  Remarques

Le type d'image est spécifié à l'aide de `options.ImageType`.
Les formats suivants sont pris en charge :
ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.


Si la largeur ou la hauteur est nulle ou si le graphique n'est pas pris en charge conformément à la liste des graphiques pris en charge, cette méthode ne fera rien.
 Prière de se référer à[Liste des graphiques pris en charge](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) pour plus de détails.


###  Voir également
* module [aspose.cells.charts](../../)
* classe [Chart](/cells/fr/python-net/aspose.cells.charts/chart)
