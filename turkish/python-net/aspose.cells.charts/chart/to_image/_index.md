---
title: to_image yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 120
url: /tr/python-net/aspose.cells.charts/chart/to_image/
is_root: false
---
##  to_image(image_file) {#str}
Grafik görüntüsünü oluşturur ve bir dosyaya kaydeder.
Dosya adının uzantısı görüntünün biçimini belirler.



```python
def to_image(self, image_file):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| image_file | str | Tam yol ile görüntü dosyası adı.|
###  Notlar

Resmin biçimi, dosya adının uzantısı kullanılarak belirtilir.
Örneğin, "dosyam.png" belirtirseniz, resim kaydedilir.
 PNG formatında. Aşağıdaki dosya uzantıları tanınır:
.bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.


Genişlik veya yükseklik sıfırsa veya tablo Desteklenen Haritalar Listesi'ne göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz.

##  to_image(image_file, image_type) {#str-aspose.cells.drawing.ImageType}
Grafik görüntüsünü oluşturur ve belirtilen görüntü tipinde bir dosyaya kaydeder.



```python
def to_image(self, image_file, image_type):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| image_file | str | Tam yol ile görüntü dosyası adı.|
| image_type | aspose.cells.drawing.ImageType | Görüntünün kaydedileceği görüntü türü.|
###  Notlar

Görüntünün türü `imageType` kullanılarak belirtilir.
 Aşağıdaki türler desteklenir:
ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.


Genişlik veya yükseklik sıfırsa veya tablo Desteklenen Haritalar Listesi'ne göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz.

##  to_image(image_file, jpeg_quality) {#str-int}
Grafik görüntüsünü oluşturur ve onu Jpeg formatında bir dosyaya kaydeder.



```python
def to_image(self, image_file, jpeg_quality):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| image_file | str | Tam yol ile görüntü dosyası adı.|
| jpeg_quality | int | JPEG kalitesi.|
###  Notlar

Genişlik veya yükseklik sıfırsa veya tablo Desteklenen Haritalar Listesi'ne göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz.

##  to_image(stream, jpeg_quality) {#io.RawIOBase-int}

Grafik görüntüsünü oluşturur ve onu Jpeg biçiminde bir akışa kaydeder.



```python
def to_image(self, stream, jpeg_quality):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| stream | io.RawIOBase | Çıkış akışı.|
| jpeg_quality | int | JPEG kalitesi.|
###  Notlar

Genişlik veya yükseklik sıfırsa veya tablo Desteklenen Haritalar Listesi'ne göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz.

##  to_image(stream, image_type) {#io.RawIOBase-aspose.cells.drawing.ImageType}

Grafik görüntüsünü oluşturur ve belirtilen biçimde bir akışa kaydeder.



```python
def to_image(self, stream, image_type):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| stream | io.RawIOBase | Çıkış akışı.|
| image_type | aspose.cells.drawing.ImageType | Görüntünün kaydedileceği görüntü türü.|
###  Notlar

Görüntünün türü `imageType` kullanılarak belirtilir.
 Aşağıdaki türler desteklenir:
ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.


Genişlik veya yükseklik sıfırsa veya tablo Desteklenen Haritalar Listesi'ne göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz.

##  to_image(image_file, options) {#str-aspose.cells.rendering.ImageOrPrintOptions}
Grafik görüntüsünü oluşturur ve bir dosyaya kaydeder.
Dosya adının uzantısı görüntünün biçimini belirler.



```python
def to_image(self, image_file, options):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| image_file | str | Tam yol ile görüntü dosyası adı.|
| options | aspose.cells.rendering.ImageOrPrintOptions | Ek görüntü oluşturma seçenekleri|
###  Notlar

Resmin biçimi, dosya adının uzantısı kullanılarak belirtilir.
Örneğin, "dosyam.png" belirtirseniz, resim kaydedilir.
 PNG formatında. Aşağıdaki dosya uzantıları tanınır:
.bmp, .gif, .png, .jpg, .jpeg, .tiff, .tif, .emf.


Genişlik veya yükseklik sıfırsa veya tablo Desteklenen Haritalar Listesi'ne göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz.
 Bakınız[Desteklenen Grafikler Listesi](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) daha fazla ayrıntı için.
###  Örnek

300 dpi ve CCITT4 sıkıştırma ile Tiff'e kaydeder.

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


300 dpi ve 80 görüntü kalitesinde Jpeg olarak kaydeder.

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
Grafik görüntüsünü oluşturur ve belirtilen biçimde bir akışa kaydeder.



```python
def to_image(self, stream, options):
    ...
```


| Parametre| Tip| Tanım|
| :- | :- | :- |
| stream | io.RawIOBase | Çıkış akışı.|
| options | aspose.cells.rendering.ImageOrPrintOptions | Ek görüntü oluşturma seçenekleri|
###  Notlar

Görüntünün türü `options.ImageType` kullanılarak belirtilir.
Aşağıdaki biçimler desteklenir:
ImageType.Bmp, ImageType.Gif, ImageType.Png, ImageType.Jpeg, ImageType.Tiff, ImageType.Emf.


Genişlik veya yükseklik sıfırsa veya tablo Desteklenen Haritalar Listesi'ne göre desteklenmiyorsa, bu yöntem hiçbir şey yapmaz.
 Bakınız[Desteklenen Grafikler Listesi](http://www.aspose.com/documentation/.net-components/aspose.cells-for-.net/converting-chart-to-image.html) daha fazla ayrıntı için.


###  Ayrıca bakınız
* modül [aspose.cells.charts](../../)
* sınıf [Chart](/cells/tr/python-net/aspose.cells.charts/chart)
