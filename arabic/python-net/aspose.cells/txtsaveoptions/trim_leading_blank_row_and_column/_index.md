---
title: trim_leading_blank_row_and_column الملكية
second_title: Aspose.Cells for Python via .NET API المراجع
description:
type: docs
weight: 220
url: /ar/python-net/aspose.cells/txtsaveoptions/trim_leading_blank_row_and_column/
is_root: false
---
##  trim_leading_blank_row_and_column الملكية

يشير إلى ما إذا كان يجب قطع الصفوف والأعمدة الفارغة البادئة مثل ما تفعله ms excel.
الافتراضي هو الصحيح.

###  ملاحظات

كما هو الحال مع القاعدة في ms excel ، لن يتم اعتبار الصف / العمود فارغًا إذا كان يحتوي على نمط مخصص ،
حتى إذا كانت لا تحتوي على بيانات خلوية.
عند الحفظ باستخدام وضع LightCells ، لا يسري هذا الخيار.
يجب على المستخدم التحكم في نطاق الإخراج بتنفيذ [TxtSaveOptions.light_cells_data_provider](/cells/ar/python-net/aspose.cells/txtsaveoptions#light_cells_data_provider)
أو عن طريق speicifing [TxtSaveOptions.export_area](/cells/ar/python-net/aspose.cells/txtsaveoptions#export_area)
###  تعريف:
```python
@property
def trim_leading_blank_row_and_column(self):
    ...
@trim_leading_blank_row_and_column.setter
def trim_leading_blank_row_and_column(self, value):
    ...
```

###  أنظر أيضا
* وحدة [aspose.cells](../../)
* فئة [TxtSaveOptions](/cells/ar/python-net/aspose.cells/txtsaveoptions)
