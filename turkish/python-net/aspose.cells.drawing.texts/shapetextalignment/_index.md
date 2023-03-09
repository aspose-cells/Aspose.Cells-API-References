---
title: ShapeTextAlignment sınıf
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 80
url: /tr/python-net/aspose.cells.drawing.texts/shapetextalignment/
is_root: false
---
##  ShapeTextAlignment sınıf
Şeklin metin hizalama ayarını temsil eder;



ShapeTextAlignment türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [is_text_wrapped](/cells/tr/python-net/aspose.cells.drawing.texts/shapetextalignment/is_text_wrapped) | Metin içeren şeklin metin kaydırmalı türünü alır ve ayarlar.|
| [rotate_text_with_shape](/cells/tr/python-net/aspose.cells.drawing.texts/shapetextalignment/rotate_text_with_shape) | Metnin şekil ile döndürülüp döndürülmediğini gösterir.|
| [text_vertical_overflow](/cells/tr/python-net/aspose.cells.drawing.texts/shapetextalignment/text_vertical_overflow) | Metin kutusunun metin dikey taşma türünü alır ve ayarlar.|
| [text_horizontal_overflow](/cells/tr/python-net/aspose.cells.drawing.texts/shapetextalignment/text_horizontal_overflow) | Metin kutusunun metin yatay taşma türünü alır ve ayarlar.|
| [rotation_angle](/cells/tr/python-net/aspose.cells.drawing.texts/shapetextalignment/rotation_angle) | Şeklin dönüşünü alır ve ayarlar.|
| [text_vertical_type](/cells/tr/python-net/aspose.cells.drawing.texts/shapetextalignment/text_vertical_type) | Metin yönünü alır ve ayarlar.|
| [auto_size](/cells/tr/python-net/aspose.cells.drawing.texts/shapetextalignment/auto_size) | Şeklin boyutunun içeriğine göre otomatik olarak ayarlanıp ayarlanmadığını gösterir.|
| [text_shape_type](/cells/tr/python-net/aspose.cells.drawing.texts/shapetextalignment/text_shape_type) | Metnin dönüştürme türünü alır ve ayarlar.|
| [top_margin_pt](/cells/tr/python-net/aspose.cells.drawing.texts/shapetextalignment/top_margin_pt) | Puan birimi cinsinden üst marjı verir|
| [bottom_margin_pt](/cells/tr/python-net/aspose.cells.drawing.texts/shapetextalignment/bottom_margin_pt) | Alt kenar boşluğunu Puan birimi cinsinden verir|
| [left_margin_pt](/cells/tr/python-net/aspose.cells.drawing.texts/shapetextalignment/left_margin_pt) | Sol kenar boşluğunu Puan birimi cinsinden verir|
| [right_margin_pt](/cells/tr/python-net/aspose.cells.drawing.texts/shapetextalignment/right_margin_pt) | Sağ kenar boşluğunu Puan birimi cinsinden verir|
| [is_auto_margin](/cells/tr/python-net/aspose.cells.drawing.texts/shapetextalignment/is_auto_margin) | Metin çerçevesinin kenar boşluğunun otomatik olup olmadığını gösterir.|
| [number_of_columns](/cells/tr/python-net/aspose.cells.drawing.texts/shapetextalignment/number_of_columns) | Sınırlayıcı dikdörtgendeki metin sütunlarının sayısını alır ve ayarlar.|



###  Örnek

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
shape = workbook.worksheets[0].shapes.add_rectangle(1, 0, 1, 0, 50, 100)
shapeTextAlignment = shape.text_body.text_alignment

```

###  Ayrıca bakınız
* modül [aspose.cells.drawing.texts](..)
