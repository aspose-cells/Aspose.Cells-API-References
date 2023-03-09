---
title: ShapeTextAlignment الدرجة
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 80
url: /ar/python-net/aspose.cells.drawing.texts/shapetextalignment/
is_root: false
---
##  ShapeTextAlignment الدرجة
يمثل إعداد محاذاة نص الشكل ؛



يكشف نوع ShapeTextAlignment الأعضاء التالية:

###  ملكيات
| ملكية| وصف|
| :- | :- |
| [is_text_wrapped](/cells/ar/python-net/aspose.cells.drawing.texts/shapetextalignment/is_text_wrapped) | الحصول على وتعيين نوع التفاف النص للشكل الذي يحتوي على نص.|
| [rotate_text_with_shape](/cells/ar/python-net/aspose.cells.drawing.texts/shapetextalignment/rotate_text_with_shape) | يشير إلى ما إذا كان يتم تدوير النص بالشكل.|
| [text_vertical_overflow](/cells/ar/python-net/aspose.cells.drawing.texts/shapetextalignment/text_vertical_overflow) | الحصول على نوع تجاوز النص العمودي لمربع النص وتعيينه.|
| [text_horizontal_overflow](/cells/ar/python-net/aspose.cells.drawing.texts/shapetextalignment/text_horizontal_overflow) | الحصول على نوع تجاوز النص الأفقي لمربع النص وتعيينه.|
| [rotation_angle](/cells/ar/python-net/aspose.cells.drawing.texts/shapetextalignment/rotation_angle) | يحصل على دوران الشكل ويضبطه.|
| [text_vertical_type](/cells/ar/python-net/aspose.cells.drawing.texts/shapetextalignment/text_vertical_type) | يحصل ويضبط اتجاه النص.|
| [auto_size](/cells/ar/python-net/aspose.cells.drawing.texts/shapetextalignment/auto_size) |يشير إلى ما إذا كان حجم الشكل يتم ضبطه تلقائيًا وفقًا لمحتواه.|
| [text_shape_type](/cells/ar/python-net/aspose.cells.drawing.texts/shapetextalignment/text_shape_type) | الحصول على نوع التحويل للنص وتعيينه.|
| [top_margin_pt](/cells/ar/python-net/aspose.cells.drawing.texts/shapetextalignment/top_margin_pt) | إرجاع الهامش الأعلى بوحدات من النقاط|
| [bottom_margin_pt](/cells/ar/python-net/aspose.cells.drawing.texts/shapetextalignment/bottom_margin_pt) | إرجاع الهامش السفلي بوحدات من النقاط|
| [left_margin_pt](/cells/ar/python-net/aspose.cells.drawing.texts/shapetextalignment/left_margin_pt) | تُرجع الهامش الأيسر بوحدات من النقاط|
| [right_margin_pt](/cells/ar/python-net/aspose.cells.drawing.texts/shapetextalignment/right_margin_pt) | تُرجع الهامش الصحيح بوحدات من النقاط|
| [is_auto_margin](/cells/ar/python-net/aspose.cells.drawing.texts/shapetextalignment/is_auto_margin) | يشير إلى ما إذا كان هامش إطار النص تلقائي.|
| [number_of_columns](/cells/ar/python-net/aspose.cells.drawing.texts/shapetextalignment/number_of_columns) | الحصول على عدد أعمدة النص وتعيينه في المستطيل المحيط.|



###  أمثلة

```python
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
shape = workbook.worksheets[0].shapes.add_rectangle(1, 0, 1, 0, 50, 100)
shapeTextAlignment = shape.text_body.text_alignment

```

###  أنظر أيضا
* وحدة [aspose.cells.drawing.texts](..)
