---
title: to_image metod
second_title: Aspose.Cells for Python via .NET API Referenser
description:
type: docs
weight: 210
url: /sv/python-net/aspose.cells.drawing/oval/to_image/
is_root: false
---
##  to_image(stream, image_type) {#io.RawIOBase-ImageType}
Skapar formbilden och sparar den i en ström i det angivna formatet.



```python
def to_image(self, stream, image_type):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| stream | io.RawIOBase | Utgångsströmmen.|
| image_type | [ImageType](/cells/sv/python-net/aspose.cells.drawing/imagetype) | Typen där bilden ska sparas.|
###  Anmärkningar

Följande format stöds:
.bmp, .gif, .jpg, .jpeg, .tiff, .emf.
###  Exempel

```python
from aspose.cells.drawing import ImageType
from io import BytesIO

imageStream = BytesIO()
shape.to_image(imageStream, ImageType.PNG)

```


##  to_image(image_file, options) {#str-aspose.cells.rendering.ImageOrPrintOptions}
Sparar formen till en fil.



```python
def to_image(self, image_file, options):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| image_file | str |  |
| options | aspose.cells.rendering.ImageOrPrintOptions |  |

###  Exempel

```python
from aspose.cells.rendering import ImageOrPrintOptions

op = ImageOrPrintOptions()
shape.to_image("exmaple.png", op)

```


##  to_image(stream, options) {#io.RawIOBase-aspose.cells.rendering.ImageOrPrintOptions}
Sparar formen till en ström.



```python
def to_image(self, stream, options):
    ...
```


| Parameter| Typ| Beskrivning|
| :- | :- | :- |
| stream | io.RawIOBase |  |
| options | aspose.cells.rendering.ImageOrPrintOptions |  |

###  Exempel

```python
from aspose.cells.rendering import ImageOrPrintOptions
from io import BytesIO

imageStream = BytesIO()
op = ImageOrPrintOptions()
shape.to_image(imageStream, op)

```



###  Se även
* modul [aspose.cells.drawing](../../)
* klass [Oval](/cells/sv/python-net/aspose.cells.drawing/oval)
