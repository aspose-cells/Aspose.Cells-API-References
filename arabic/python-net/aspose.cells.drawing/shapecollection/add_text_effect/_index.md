---
title: طريقة add_text_effect
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 330
url: /ar/python-net/aspose.cells.drawing/shapecollection/add_text_effect/
is_root: false
---
##  add_text_effect(effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width) {#MsoPresetTextEffect-str-str-int-bool-bool-int-int-int-int-int-int}
يُدرج كائن WordArt.


###  عائدات

إرجاع كائن الشكل الذي يمثل كائن WordArt الجديد.


```python
def add_text_effect(self, effect, text, font_name, size, font_bold, font_italic, upper_left_row, top, upper_left_column, left, height, width):
    ...
```


| معامل| يكتب| وصف|
| :- | :- | :- |
| effect | [MsoPresetTextEffect](/cells/ar/python-net/aspose.cells.drawing/msopresettexteffect) | نوع تأثير النص المعين مسبقًا mso.|
| text | str | نص WordArt.|
| font_name | str | اسم الخط.|
| size | int | حجم الخط|
| font_bold | bool | يشير إلى ما إذا كان الخط غامقًا أم لا.|
| font_italic | bool | يشير إلى ما إذا كان الخط مائلاً.|
| upper_left_row | int | فهرس الصف العلوي الأيسر.|
| top | int | يمثل الإزاحة الرأسية للشكل من صفه الأيسر ، بوحدة البكسل.|
| upper_left_column | int | فهرس العمود الأيسر العلوي.|
| left | int |يمثل الإزاحة الأفقية للشكل من العمود الأيسر ، بوحدة البكسل.|
| height | int | يمثل ارتفاع الشكل بوحدة البكسل.|
| width | int | يمثل عرض الشكل بوحدة البكسل.|

###  مثال

```python
from aspose.cells.drawing import MsoPresetTextEffect

# add a WordArt
wordArt1 = shapes.add_text_effect(MsoPresetTextEffect.TEXT_EFFECT10, "WordArt", "arial", 18, False, False, 3, 0, 3, 0, 200, 50)

```



###  أنظر أيضا
* وحدة [aspose.cells.drawing](../../)
* فئة [ShapeCollection](/cells/ar/python-net/aspose.cells.drawing/shapecollection)
