---
title: TextEffectFormat sınıfı
second_title: Aspose.Cells for Python via .NET API Referanslar
description:
type: docs
weight: 700
url: /tr/python-net/aspose.cells.drawing/texteffectformat/
is_root: false
---
##  TextEffectFormat sınıfı
WordArt nesnelerine uygulanan özellikleri ve yöntemleri içerir.



TextEffectFormat türü aşağıdaki üyeleri gösterir:

###  Özellikler
| Mülk| Tanım|
| :- | :- |
| [text](/cells/tr/python-net/aspose.cells.drawing/texteffectformat/text) | WordArt'taki metin.|
| [font_name](/cells/tr/python-net/aspose.cells.drawing/texteffectformat/font_name) | WordArt'ta kullanılan yazı tipinin adı.|
| [font_bold](/cells/tr/python-net/aspose.cells.drawing/texteffectformat/font_bold) | Yazı tipinin kalın olup olmadığını gösterir.|
| [font_italic](/cells/tr/python-net/aspose.cells.drawing/texteffectformat/font_italic) | Yazı tipinin italik olup olmadığını gösterir.|
| [rotated_chars](/cells/tr/python-net/aspose.cells.drawing/texteffectformat/rotated_chars) | Doğruysa, belirtilen WordArt'taki karakterler, WordArt'ın sınırlayıcı şekline göre 90 derece döndürülür.|
| [font_size](/cells/tr/python-net/aspose.cells.drawing/texteffectformat/font_size) | WordArt'ta kullanılan yazı tipinin boyutu (punto olarak).|
| [preset_shape](/cells/tr/python-net/aspose.cells.drawing/texteffectformat/preset_shape) | Önceden ayarlanmış şekil türünü alır ve ayarlar.|


###  Yöntemler
| Yöntem| Tanım|
| :- | :- |
| [set_text_effect(effect)](/cells/tr/python-net/aspose.cells.drawing/texteffectformat/set_text_effect/#MsoPresetTextEffect) | Önceden ayarlanmış metin efektini ayarlar.|



###  Örnek

```python
from aspose.cells import Workbook
from aspose.cells.drawing import MsoPresetTextEffect

# Instantiating a Workbook object
workbook = Workbook()
shapes = workbook.worksheets[0].shapes
shapes.add_text_effect(MsoPresetTextEffect.TEXT_EFFECT1, "Aspose", "Arial", 30, False, False, 0, 0, 0, 0, 100, 200)
textEffectFormat = shapes[0].text_effect
textEffectFormat.set_text_effect(MsoPresetTextEffect.TEXT_EFFECT10)
workbook.save("Book1.xls")

```

###  Ayrıca bakınız
* modül [aspose.cells.drawing](..)
