---
title: TextEffectFormat الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 700
url: /ar/python-net/aspose.cells.drawing/texteffectformat/
is_root: false
---
##  TextEffectFormat الدرجة
يحتوي على الخصائص والأساليب التي تنطبق على كائنات WordArt.



يكشف نوع TextEffectFormat الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [text](/cells/ar/python-net/aspose.cells.drawing/texteffectformat/text) | النص الموجود في WordArt.|
| [font_name](/cells/ar/python-net/aspose.cells.drawing/texteffectformat/font_name) | اسم الخط المستخدم في WordArt.|
| [font_bold](/cells/ar/python-net/aspose.cells.drawing/texteffectformat/font_bold) | يشير إلى ما إذا كان الخط غامقًا أم لا.|
| [font_italic](/cells/ar/python-net/aspose.cells.drawing/texteffectformat/font_italic) | يشير إلى ما إذا كان الخط مائلاً.|
| [rotated_chars](/cells/ar/python-net/aspose.cells.drawing/texteffectformat/rotated_chars) | إذا كان هذا صحيحًا ، فسيتم تدوير الأحرف في WordArt المحدد بمقدار 90 درجة بالنسبة إلى الشكل المحيط في WordArt.|
| [font_size](/cells/ar/python-net/aspose.cells.drawing/texteffectformat/font_size) | حجم الخط (بالنقاط) المستخدم في WordArt.|
| [preset_shape](/cells/ar/python-net/aspose.cells.drawing/texteffectformat/preset_shape) | الحصول على نوع الشكل المحدد مسبقًا وتعيينه.|


###  طُرق
| طريقة| وصف|
| :- | :- |
| [set_text_effect(effect)](/cells/ar/python-net/aspose.cells.drawing/texteffectformat/set_text_effect/#MsoPresetTextEffect) | يضبط تأثير النص المعين مسبقًا.|



###  أمثلة

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

###  أنظر أيضا
* وحدة [aspose.cells.drawing](..)
