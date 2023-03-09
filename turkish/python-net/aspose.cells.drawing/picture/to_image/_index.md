---
title: to_image yöntemi
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 230
url: /tr/python-net/aspose.cells.drawing/picture/to_image/
is_root: false
---
##  to_image(stream, image_type) {#io.RawIOBase-ImageType}
Şekil görüntüsünü oluşturur ve belirtilen biçimde bir akışa kaydeder.



```python
def to_image(self, stream, image_type):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| stream | io.RawIOBase | Çıkış akışı.|
| image_type | [ImageType](/cells/tr/python-net/aspose.cells.drawing/imagetype) | Görüntünün kaydedileceği tür.|
###  Notlar

Aşağıdaki biçimler desteklenir:
.bmp, .gif, .jpg, .jpeg, .tiff, .emf.
###  örnekler

```python
from aspose.cells.drawing import ImageType
from io import BytesIO

imageStream = BytesIO()
shape.to_image(imageStream, ImageType.PNG)

```


##  to_image(image_file, options) {#str-aspose.cells.rendering.ImageOrPrintOptions}
Şekli bir dosyaya kaydeder.



```python
def to_image(self, image_file, options):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| image_file | str |  |
| options | aspose.cells.rendering.ImageOrPrintOptions |  |

###  örnekler

```python
from aspose.cells.rendering import ImageOrPrintOptions

op = ImageOrPrintOptions()
shape.to_image("exmaple.png", op)

```


##  to_image(stream, options) {#io.RawIOBase-aspose.cells.rendering.ImageOrPrintOptions}
Şekli bir akışa kaydeder.



```python
def to_image(self, stream, options):
    ...
```


| parametreler| Tip| Tanım|
| :- | :- | :- |
| stream | io.RawIOBase |  |
| options | aspose.cells.rendering.ImageOrPrintOptions |  |

###  örnekler

```python
from aspose.cells.rendering import ImageOrPrintOptions
from io import BytesIO

imageStream = BytesIO()
op = ImageOrPrintOptions()
shape.to_image(imageStream, op)

```



###  Ayrıca bakınız
* modül [aspose.cells.drawing](../../)
* sınıf [Picture](/cells/tr/python-net/aspose.cells.drawing/picture)
