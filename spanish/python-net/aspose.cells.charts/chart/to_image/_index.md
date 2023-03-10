---
title: to_image método
second_title: Aspose.Cells for Python via .NET API Referencias
description:
type: docs
weight: 120
url: /es/python-net/aspose.cells.charts/chart/to_image/
is_root: false
---
##  to_image(image_file) {#str}
Crea la imagen del gráfico y la guarda en un archivo.
La extensión del nombre del archivo determina el formato de la imagen.



```python
def to_image(self, image_file):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| image_file | str | El nombre del archivo de imagen con la ruta completa.|
###  Observaciones

El formato de la imagen se especifica utilizando la extensión del nombre del archivo.
Por ejemplo, si especifica "miarchivo.png", la imagen se guardará
 en el formato PNG. Se reconocen las siguientes extensiones de archivo:
.bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.


Si el ancho o la altura es cero o el gráfico no es compatible de acuerdo con la Lista de gráficos compatibles, este método no hará nada.

##  to_image(image_file, image_type) {#str-aspose.cells.drawing.ImageType}
Crea la imagen del gráfico y la guarda en un archivo con el tipo de imagen especificado.



```python
def to_image(self, image_file, image_type):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| image_file | str | El nombre del archivo de imagen con la ruta completa.|
| image_type | aspose.cells.drawing.ImageType | El tipo de imagen en el que guardar la imagen.|
###  Observaciones

El tipo de imagen se especifica utilizando `imageType`.
 Se admiten los siguientes tipos:
ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.


Si el ancho o la altura es cero o el gráfico no es compatible de acuerdo con la Lista de gráficos compatibles, este método no hará nada.

##  to_image(image_file, jpeg_quality) {#str-int}
Crea la imagen del gráfico y la guarda en un archivo en formato Jpeg.



```python
def to_image(self, image_file, jpeg_quality):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| image_file | str | El nombre del archivo de imagen con la ruta completa.|
| jpeg_quality | int | Calidad JPEG.|
###  Observaciones

Si el ancho o la altura es cero o el gráfico no es compatible de acuerdo con la Lista de gráficos compatibles, este método no hará nada.

##  to_image(stream, jpeg_quality) {#io.RawIOBase-int}

Crea la imagen del gráfico y la guarda en una secuencia en formato Jpeg.



```python
def to_image(self, stream, jpeg_quality):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| stream | io.RawIOBase | El flujo de salida.|
| jpeg_quality | int | Calidad JPEG.|
###  Observaciones

Si el ancho o la altura es cero o el gráfico no es compatible de acuerdo con la Lista de gráficos compatibles, este método no hará nada.

##  to_image(stream, image_type) {#io.RawIOBase-aspose.cells.drawing.ImageType}

Crea la imagen del gráfico y la guarda en una secuencia en el formato especificado.



```python
def to_image(self, stream, image_type):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| stream | io.RawIOBase | El flujo de salida.|
| image_type | aspose.cells.drawing.ImageType | El tipo de imagen en el que guardar la imagen.|
###  Observaciones

El tipo de imagen se especifica utilizando `imageType`.
 Se admiten los siguientes tipos:
ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.


Si el ancho o la altura es cero o el gráfico no es compatible de acuerdo con la Lista de gráficos compatibles, este método no hará nada.

##  to_image(image_file, options) {#str-aspose.cells.rendering.ImageOrPrintOptions}
Crea la imagen del gráfico y la guarda en un archivo.
La extensión del nombre del archivo determina el formato de la imagen.



```python
def to_image(self, image_file, options):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| image_file | str | El nombre del archivo de imagen con la ruta completa.|
| options | aspose.cells.rendering.ImageOrPrintOptions | Opciones adicionales de creación de imágenes|
###  Observaciones

El formato de la imagen se especifica utilizando la extensión del nombre del archivo.
Por ejemplo, si especifica "miarchivo.png", la imagen se guardará
 en el formato PNG. Se reconocen las siguientes extensiones de archivo:
.bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.


Si el ancho o la altura es cero o el gráfico no es compatible de acuerdo con la Lista de gráficos compatibles, este método no hará nada.
 Por favor refiérase a[Lista de gráficos admitidos](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html)para más detalles.
###  Ejemplo

Guarda en Tiff con 300 dpi y compresión CCITT4.

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


Guarda en Jpeg con 300 ppp y calidad de imagen 80.

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
Crea la imagen del gráfico y la guarda en una secuencia en el formato especificado.



```python
def to_image(self, stream, options):
    ...
```


| Parámetro| Tipo| Descripción|
| :- | :- | :- |
| stream | io.RawIOBase | El flujo de salida.|
| options | aspose.cells.rendering.ImageOrPrintOptions | Opciones adicionales de creación de imágenes|
###  Observaciones

El tipo de imagen se especifica utilizando `options.ImageType`.
 Se admiten los siguientes formatos:
ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.


Si el ancho o la altura es cero o el gráfico no es compatible de acuerdo con la Lista de gráficos compatibles, este método no hará nada.
 Por favor refiérase a[Lista de gráficos admitidos](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html)para más detalles.


###  Ver también
* módulo [aspose.cells.charts](../../)
* clase [Chart](/cells/es/python-net/aspose.cells.charts/chart)
